# EasyToggle
EasyToggle是一个Kotlin写的轻量级的开关控件，只有一个文件，默认设置下它的行为跟ios的开关控件是一毛一样的，当然你也可以通过它提供的属性自己设计开关的外观。当手指在不同的范围内触摸时，EasyToggle会有不同的表现，这样的用户体验还是挺不错的。

## 演示
![easytoggle](https://github.com/huzenan/EasyToggle/blob/master/screeshots/easytoggle.gif) 

## 用法
>layout

布局中非常简单，如果你正好想要的是一个ios效果的开关，那你在布局文件中无需做任何设置。
```xml
    <com.hzn.lib.EasyToggle
        android:id="@+id/et"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        />
```
>Activity

可以非常简单地用lambda表达式来设置监听
```kotlin
    et.setOnToggledListener {
        tv.text = if (it) "on" else "off"
    }
```

## 属性
| 属性名               | 描述           |
| ------------------- | ------------- |
| etLength            | 按钮的扩展长度（不包含半径radius） |
| etRadius            | 按钮的半径长度 |
| etRange             | 使EasyToggle改变行为的限定范围 |
| etBgOffColor        | 关闭时的背景颜色 |
| etBgOnColor         | 打开时的背景颜色 |
| etBgStrokeWidth     | 背景的边框宽度 |
| etBgTopColor        | 背景上的另一层的颜色 |
| etButtonColor       | 按钮的颜色 |
| etButtonStrokeColor | 按钮边框的颜色 |
| etButtonStrokeWidth | 按钮边框的宽度 |
| etShadowOffsetY     | 按钮影子在Y方向上的偏移值，大于0 |
