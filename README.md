<h1 align="center">Pretty Logger</h1></br>
<p align="center">🌈 a Pretty Log Library for Android Studio 🎉</p></br>
<p align="center">
  <a href="https://github.com/sungbin5304/PrettyLogger/blob/master/LICENSE"><img alt="License" src="https://img.shields.io/badge/License-Apache2-blue"/></a>
  <a href="https://github.com/sungbin5304/PrettyLogger"><img alt="Title" src="https://img.shields.io/badge/Pretty-LOGGER-ff69b4"/></a>
</p><br>

<p align="center">
<img src="https://raw.githubusercontent.com/sungbin5304/PrettyLogger/master/images/log.png"/>
</p>

-----

# Download
You can download at [this](https://github.com/sungbin5304/AndroidUtils/blob/master/README.md#logutils-more-guide) page.

# LogUtils
## Logging with Default Tag
``` Kotlin
- w(any: Any?)
- v(any: Any?)
- d(any: Any?)
- e(any: Any?)
- i(any: Any?)
```

## Logging with Custom Tag
``` Kotlin
- w(tag: String, any: Any?)
- v(tag: String, any: Any?)
- d(tag: String, any: Any?)
- e(tag: String, any: Any?)
- i(tag: String, any: Any?)
```

# Option
## Default Tag
Default tag is `TAG`.<br>
You can set your Tag with `setTag(tag: String)` method.

## ShowLogControl
You can control show log with `showLog(showLog: Boolean)` method.

# Tip
## 1. PrettyLogger is supported `Iterable`, `Array` and `Map` logging.
``` Kotlin
val map = HashMap<String, String>()
map["A"] = "BCD"
map["E"] = "FGH"
map["I"] = "JKL"
LogUtils.d("Map Content", map)
LogUtils.i("Iterable Content", arrayListOf("T", "", "E", "", "S", "T", "", "above data is empty value."))
LogUtils.e(null)
LogUtils.w("This is my Pretty Log.")
LogUtils.setTag("Custom Tag")
LogUtils.v("Change Tag.")
```
![preview](https://github.com/sungbin5304/PrettyLogger/blob/master/images/PrettyLogger.png)

## 2. Change Android Studio logcat color.
1. File -> Settings -> Search `android logcat`
2. Unchecked `Inherit values from:`
3. Input your logcat color.
### Suggest logcat color
Debug : `6897BB`<br>
Info : `6A8759`<br>
Warn : `BBB529`<br>
Error : `FF6B68`<br>
Assert : `9876AA`<br>
