---
title: "FontResolveEventArgs"
second_title: "Aspose.Tasks for Java API 参考"
description: "提供在字体解析时调用的回调的参数。"
type: docs
weight: 99
url: /zh/java/com.aspose.tasks/fontresolveeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public final class FontResolveEventArgs extends System.EventArgs
```

提供在字体解析时调用的回调的参数。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getRequestedFontName()](#getRequestedFontName--) | 获取请求的字体名称。 |
| [getResolvedFontName()](#getResolvedFontName--) | 获取已解析字体的名称。 |
| [setResolvedFontName(String value)](#setResolvedFontName-java.lang.String-) | 设置已解析字体的名称。 |
### getRequestedFontName() {#getRequestedFontName--}
```
public final String getRequestedFontName()
```


获取请求的字体名称。

**Returns:**
java.lang.String - 请求的字体名称。
### getResolvedFontName() {#getResolvedFontName--}
```
public final String getResolvedFontName()
```


获取已解析字体的名称。可设置以控制用于渲染视图的字体。

**Returns:**
java.lang.String - 如果找到字体则为请求的字体名称，或为回退字体的名称，若未找到则为 null。
### setResolvedFontName(String value) {#setResolvedFontName-java.lang.String-}
```
public final void setResolvedFontName(String value)
```


设置已解析字体的名称。可设置以控制用于渲染视图的字体。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 已解析字体的名称。 |

