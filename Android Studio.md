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


### FileOutputStream
    该类用来创建一个文件并向文件中写数据。如果该流在打开文件进行输出前，目标文件不存在，那么该流会创建该文件。
    

### FileOutputStream和openFileOutput()
#### FileOutputStream
    该类用来创建一个文件并向文件中写数据。如果该流在打开文件进行输出前，目标文件不存在，那么该流会创建该文件。
#### openFileOutput()
    openFileOutput()方法可以用于把数据输出到文件中。openFileOutput()返回的是一个FileOutputStream对象，得到了对象之后
    就可以使用Java流的方式将数据写入到文件中了。
    openFileOutput()第一参数用于指定文件名称，不能包含路径分隔符"/"，如果文件不存在，Android会自动创建它。创建的文件保存
    在/data/data/<package name>/files目录；
    openFileOutput()第二参数是文件的操作模式：MODE_PRIVATE覆盖内容，MODE_APPEND追加内容
#### 例：
    FileOutputStream out = null;
    out = OpenFileOutput("data",Context.MODE_PRIVATE);
    
### BufferedWriter字符缓冲输出流
    BufferedWriter writer = null;
    writer = new BufferedWriter(new OutputStreamWriter(out));
    OutputStreamWriter类是Writer类的子类，是从字符流到字节流的桥梁。
    
        
