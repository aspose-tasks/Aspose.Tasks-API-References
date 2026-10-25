---
title: "FontDescriptor"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示字体信息。"
type: docs
weight: 96
url: /zh/java/com.aspose.tasks/fontdescriptor/
---

**Inheritance:**
java.lang.Object
```
public final class FontDescriptor
```

表示字体信息。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [FontDescriptor(String fontFamily, float size)](#FontDescriptor-java.lang.String-float-) | 使用指定的字体族和大小初始化 [FontDescriptor](../../com.aspose.tasks/fontdescriptor) 类的新实例。 |
| [FontDescriptor(String fontFamily, float size, int style)](#FontDescriptor-java.lang.String-float-int-) | 使用指定的字体族、大小和样式初始化 [FontDescriptor](../../com.aspose.tasks/fontdescriptor) 类的新实例。 |
| [FontDescriptor(FontDescriptor font, int style)](#FontDescriptor-com.aspose.tasks.FontDescriptor-int-) | 使用指定的字体和样式初始化 [FontDescriptor](../../com.aspose.tasks/fontdescriptor) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getFontFamily()](#getFontFamily--) | 获取字体族的名称。 |
| [getSize()](#getSize--) | 获取字体的大小。 |
| [getStyle()](#getStyle--) | 获取字体的样式。 |
### FontDescriptor(String fontFamily, float size) {#FontDescriptor-java.lang.String-float-}
```
public FontDescriptor(String fontFamily, float size)
```


使用指定的字体族和大小初始化 [FontDescriptor](../../com.aspose.tasks/fontdescriptor) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontFamily | java.lang.String | 字体族的名称。 |
| 大小 | float | 字体的大小。 |

### FontDescriptor(String fontFamily, float size, int style) {#FontDescriptor-java.lang.String-float-int-}
```
public FontDescriptor(String fontFamily, float size, int style)
```


使用指定的字体族、大小和样式初始化 [FontDescriptor](../../com.aspose.tasks/fontdescriptor) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontFamily | java.lang.String | 字体族的名称。 |
| 大小 | float | 字体的大小。 |
| 样式 | int | 字体的样式。 |

### FontDescriptor(FontDescriptor font, int style) {#FontDescriptor-com.aspose.tasks.FontDescriptor-int-}
```
public FontDescriptor(FontDescriptor font, int style)
```


使用指定的字体和样式初始化 [FontDescriptor](../../com.aspose.tasks/fontdescriptor) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | 要复制的 [FontDescriptor](../../com.aspose/tasks/fontdescriptor) 实例。 |
| 样式 | int | 字体的样式。 |

### getFontFamily() {#getFontFamily--}
```
public final String getFontFamily()
```


获取字体族的名称。

**Returns:**
java.lang.String - 字体系列的名称。
### getSize() {#getSize--}
```
public final float getSize()
```


获取字体的大小。

**Returns:**
float - 字体的大小。
### getStyle() {#getStyle--}
```
public final int getStyle()
```


获取字体的样式。

**Returns:**
int - 字体的样式。
