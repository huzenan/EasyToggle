# EasyToggle

([ 我爱中文 ](./README_CN.md))

A light toggle view for Android in Kotlin, with only 1 file, it acts like ios toggle style in default settings, also you can design it using all the given attributes. The toggle view acts differently while touching different ranges around the button, it performs good experience for user.

## ScreenShots
![easytoggle](https://github.com/huzenan/EasyToggle/blob/master/screeshots/easytoggle.gif) 

## Usage
>layout

The layout is very simple, if you want exactly a ios style toggle, nothing need to be set in your layout file.
```xml
    <com.hzn.lib.EasyToggle
        android:id="@+id/et"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        />
```
>Activity

Using lambda, setting the listener is also very easy.
```kotlin
    et.setOnToggledListener {
        tv.text = if (it) "on" else "off"
    }
```

## Attributes
| name                | description   |
| ------------------- | ------------- |
| etLength            | button extensional length(without raidus) |
| etRadius            | radius of the button |
| etRange             | range that changes the acting of the toggle view |
| etBgOffColor        | background color when off |
| etBgOnColor         | background color when on |
| etBgStrokeWidth     | background stroke width |
| etBgTopColor        | color above the backgroud |
| etButtonColor       | color of the button |
| etButtonStrokeColor | color of stroke of the button |
| etButtonStrokeWidth | stroke width of the button |
| etShadowOffsetY     | offsetY of shadow, greater than 0 |
