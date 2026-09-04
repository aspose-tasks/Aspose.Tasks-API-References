---
title: "FontSettings"
second_title: "Aspose.Tasks for Java API 参考"
description: "指定在渲染项目视图时使用的字体设置。"
type: docs
weight: 101
url: /zh/java/com.aspose.tasks/fontsettings/
---

**Inheritance:**
java.lang.Object
```
public final class FontSettings
```

指定在渲染项目视图时使用的字体设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [FontSettings()](#FontSettings--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDefaultFontName()](#getDefaultFontName--) | 获取用于渲染的默认（或回退）字体。 |
| [getFontResolveCallback()](#getFontResolveCallback--) | 获取可用于自定义已解析字体的回调。 |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | 获取指示是否必须在渲染时使用默认字体的值。 |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | 设置用于渲染的默认（或回退）字体。 |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | 设置 Aspose.Tasks 在渲染项目视图时查找 TrueType 字体的文件夹。 |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | 设置可用于自定义已解析字体的回调。 |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | 设置指示是否必须在渲染时使用默认字体的值。 |
### FontSettings() {#FontSettings--}
```
public FontSettings()
```


### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


获取用于渲染的默认（或回退）字体。

**Returns:**
java.lang.String - 用于渲染的默认（或回退）字体。
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


获取可用于自定义已解析字体的回调。

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


获取指示是否必须在渲染时使用默认字体的值。

--------------------

当值为 False 且指定了 DefaultFontName 时，渲染引擎将使用 DefaultFontName 指定的字体作为回退字体。否则，将使用已安装的 'Arial'（如果存在）或 'Generic Sans Serif' 字体作为回退字体。当文本样式引用当前操作系统未安装的字体时，回退字体将在项目视图的渲染过程中使用。若需更精细地控制字体解析，可使用 `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) 回调。

**Returns:**
boolean - 指示是否必须在渲染时使用默认字体的值。
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


设置用于渲染的默认（或回退）字体。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 用于渲染的默认（或回退）字体。 |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public final void setFontFolders(String[] fontFolders, boolean recursive)
```


设置 Aspose.Tasks 在渲染项目视图时查找 TrueType 字体的文件夹。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontFolders | java.lang.String[] | 包含 TrueType 字体的文件夹数组。 |
| recursive | boolean | 如果为 true，指定的文件夹将被递归扫描。 |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


设置可用于自定义已解析字体的回调。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | 可用于自定义已解析字体的回调。 |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


设置指示是否必须在渲染时使用默认字体的值。

--------------------

当值为 False 且指定了 DefaultFontName 时，渲染引擎将使用 DefaultFontName 指定的字体作为回退字体。否则，将使用已安装的 'Arial'（如果存在）或 'Generic Sans Serif' 字体作为回退字体。当文本样式引用当前操作系统未安装的字体时，回退字体将在项目视图的渲染过程中使用。若需更精细地控制字体解析，可使用 `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) 回调。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示在渲染时是否必须使用默认字体的值。 |

