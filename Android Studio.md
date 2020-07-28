## Android Studio 操作指令

    格式化代码：ctrl+alt+L
    重写方法：ctrl+O

### android:layout_gravity和android:gravity
    android:gravity是对元素本身说的，指的是文字在控件中的对齐方式。或者字view在父view中的对其方式(在父view中设置)。
    android:layout_gravity是LinearLayout的属性，用于指定控件在布局中的对齐方式，当LinearLayout的排列方式是horizontal时，只有在垂直方向上的对齐方式才会生效，因为此时水平方向的长度是不固定的，每添加一个控件，水平方向上的长度都会改变，因而无法指定该方向上的对其方式。同样的道理，当LinearLayout的排列方式为vertical时，只有水平方向上的对其方式才会生效。

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/hc951129/Android-Studio/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
