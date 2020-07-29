 ## Android Studio 操作指令

    格式化代码：ctrl+alt+L
    重写方法：ctrl+O
    在整个项目中搜寻(Find in Path)：ctrl+shift+F

### android:layout_gravity和android:gravity
    android:gravity是对元素本身说的，指的是文字在控件中的对齐方式。或者字view在父view中的对其方式(在父view中设置)。
    android:layout_gravity是LinearLayout的属性，用于指定控件在布局中的对齐方式，当LinearLayout的排列方式是horizontal时，
    只有在垂直方向上的对齐方式才会生效，因为此时水平方向的长度是不固定的，每添加一个控件，水平方向上的长度都会改变，因而无法
    指定该方向上的对其方式。同样的道理，当LinearLayout的排列方式为vertical时，只有水平方向上的对其方式才会生效。


### File类中的list和listFiles方法
    list()方法是返回某个目录下的所有文件和目录的文件名，返回的是String数组
    listFiles()方法返回的是某个目录下所有文件和目录的绝对路径，返回的是File数组

### TextView添加滚动条
    在xml文件中的TextView中添加：android:scrollbars="vertical"(垂直滚动)
    在java文件中添加：textView.setMovementMethod(ScrollingMovementMethod.getInstance());
