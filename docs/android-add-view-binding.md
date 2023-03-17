# 如何在 Android Gradle 项目中添加视图绑定

> 原文：<https://www.xda-developers.com/android-add-view-binding/>

大多数 Android 开发人员可能都熟悉经典的`findViewById()`方法。将 XML 布局中的一个视图的 ID 传递给它，它将返回对该视图的放大版本的引用。这都是假设您传递了正确的 ID，并且视图确实存在。`findViewById()`没有内置检查来防止您试图检索您无法检索的视图。输入视图绑定。

视图绑定自动为每个布局 XML 生成一个绑定类，而不是在每个视图上使用`findViewById()`。每个带有 ID 的视图都会自动添加到类中，因此您可以直接引用它们。

向 Android Gradle 项目添加视图绑定非常简单。

## Gradle Setup

在 Gradle 中，视图绑定是在模块级别启用的。如果您有多个模块，您需要为每个模块单独启用它。

在模块级`build.gradle`的`android`块中，添加启用视图绑定的选项。

```
 android {
    ...

    buildFeatures {
        viewBinding true
    }
} 
```

可能会有一个关于非法访问的警告，但那是一个 lint bug，可以安全地忽略。

将启用同步项目和视图绑定。就这么简单。

## 使用视图绑定

使用视图绑定有几种方法，但是在这之前，让我们先讨论一下绑定类是如何生成的。

### 类名语法

假设您有一个名为`some_layout.xml`的布局 XML。其对应的绑定类将被命名为`SomeLayoutBinding`。这种模式适用于所有文件。

每个单词(文件名中用下划线分隔)都将大写，下划线将被删除。“绑定”然后被添加到末尾。

### 用现有视图实例化

如果您已经扩展了布局文件，并且有了对布局根的引用，那么您可以告诉视图绑定类使用现有的布局。

**锅炉**:

```
 val binding = SomeLayoutBinding.bind(someLayoutRoot ) 
```

**Java** :

```
 SomeLayoutBinding binding = SomeLayoutBinding.bind(someLayoutRoot ); 
```

例如，如果您想在一个片段中使用 binding 类，它看起来就像这样。

**锅炉**:

```
 class SomeFragment : Fragment(R.layout.some_layout) {

    private val binding by lazy { SomeLayoutBinding.bind(view) }

    override fun onViewCreated(view: View, savedInstanceState: Bundle?) {
        super.onViewCreated(view, savedInstanceState)

    }
} 
```

**Java** :

```
 public class SomeFragment extends Fragment {
    private SomeLayoutBinding binding = null;

    public SomeFragment() {
        super(R.layout.some_layout);
    }

    @Override
    public void onViewCreated(View view, Bundle savedInstanceState) {
        super.onViewCreated(view, savedInstanceState);

        binding = SomeLayoutBinding.bind(view);
    }
} 
```

### 用新视图实例化

binding 类也可以为您放大布局。

**锅炉**:

```
 val binding = SomeLayoutBinding.inflate(layoutInflater ) 
```

**Java** :

```
 SomeLayoutBinding binding = SomeLayoutBinding.inflate(layoutInflater ); 
```

这个方法在片段和活动中都有用。

一个**示例片段**看起来像下面这样。

**锅炉**:

```
 class SomeFragment : Fragment() {
    private val binding by lazy { SomeLayoutBinding.inflate(LayoutInflater.from(requireContext())) }

    override fun onCreateView(inflater: LayoutInflater, container: ViewGroup?, savedInstanceState: Bundle?) {

        return binding.root
    }
} 
```

**Java** :

```
 public class SomeFragment extends Fragment {
    private SomeLayoutBinding binding = null;

    @Override
    public void onCreateView(LayoutInflater inflater, ViewGroup container, Bundle savedInstanceState) {

        binding = SomeLayoutBinding.inflate(inflater);

        return binding.getRoot();
    }
} 
```

一个**示例活动**如下所示。

**锅炉**:

```
 class SomeActivity : AppCompatActivity() {
    private val binding by lazy { SomeLayoutBinding.inflate(layoutInflater) }

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)

        setContentView(binding.root)
    }
} 
```

**Java** :

```
 public class SomeActivity extends AppCompatActivity {
    private SomeLayoutBinding binding = null;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);

        binding = SomeLayoutBinding.inflate(getLayoutInflater());

        setContentView(binding.getRoot());
    }
} 
```

### 参考视图

既然视图绑定类已经设置好并可以使用了，是时候实际使用它了。

假设`some_layout.xml`的内容如下:

```
 <LinearLayout
    android:
    ...>
    <FrameLayout
        android:
        ...
        />
    <ImageView
        android:
        ...
        />
    <LinearLayout
        android:
        ...>
        <ImageView
            android:
            ...
            />
    </LinearLayout>
</LinearLayout> 
```

代码中有很多 id 可以引用。但是只要实例化了绑定类，引用就很容易了。

在 Kotlin 中，视图由匹配其 id 的变量引用，只是有些变化。下划线被删除，产生的字符串是驼峰式大小写。例如，要从代码中引用`some_frame_layout`，您可以使用`binding.someFrameLayout`。`someFrameLayout`变量将是 FrameLayout 的一个实例。

```
 val someFrameLayout: FrameLayout = binding.someFrameLayout 
```

在 Java 中，视图由匹配其 id 的 getter 方法引用，格式类似于 Kotlin。例如，要引用`some_frame_layout`，你可以使用`binding.getSomeFrameLayout()`。该方法将返回 FrameLayout 的一个实例。

```
 FrameLayout someFrameLayout = binding.getSomeFrameLayout(); 
```

视图引用在绑定中也被展平。引用`inner_imageview`与引用`some_frame_layout`相同。

## 结论

我相信你可以看到，Android 中的视图绑定既容易实现又容易使用。很多时候比`findViewById()`好用。

关于实现视图绑定的更多细节，以及一些例子，[查看 Google 的官方文档](https://developer.android.com/topic/libraries/view-binding)。