---
title: "TextStyle"
second_title: "Aspose.Tasks for Java API 参考"
description: "更改项目视图中项目的文本视觉样式。"
type: docs
weight: 315
url: /zh/java/com.aspose.tasks/textstyle/
---

**Inheritance:**
java.lang.Object
```
public class TextStyle
```

更改项目视图中项目的文本视觉样式。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TextStyle()](#TextStyle--) | 使用默认设置初始化 [TextStyle](../../com.aspose.tasks/textstyle) 类的一个新实例。 |
| [TextStyle(float fontSize, int fontStyle)](#TextStyle-float-int-) | 使用默认字体以及指定的字体大小和样式初始化 [TextStyle](../../com.aspose.tasks/textstyle) 类的一个新实例。 |
| [TextStyle(int fontStyle)](#TextStyle-int-) | 使用默认字体和指定的字体样式初始化 [TextStyle](../../com.aspose.tasks/textstyle) 类的一个新实例。 |
| [TextStyle(FontDescriptor font)](#TextStyle-com.aspose.tasks.FontDescriptor-) | 使用指定的字体设置初始化 [TextStyle](../../com.aspose.tasks/textstyle) 类的一个新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getBackgroundColor()](#getBackgroundColor--) | 获取文本样式的背景颜色。 |
| [getBackgroundPattern()](#getBackgroundPattern--) | 获取文本样式的背景图案。 |
| [getColor()](#getColor--) | 获取文本的颜色。 |
| [getFont()](#getFont--) | 获取文本样式的字体。 |
| [getItemType()](#getItemType--) | 获取文本样式的 [TextItemType](../../com.aspose.tasks/textitemtype)。 |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | 设置文本样式的背景颜色。 |
| [setBackgroundPattern(int value)](#setBackgroundPattern-int-) | 设置文本样式的背景图案。 |
| [setColor(Color value)](#setColor-java.awt.Color-) | 设置文本的颜色。 |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | 设置文本样式的字体。 |
| [setItemType(int value)](#setItemType-int-) | 设置文本样式的 [TextItemType](../../com.aspose.tasks/textitemtype)。 |
### TextStyle() {#TextStyle--}
```
public TextStyle()
```


使用默认设置初始化 [TextStyle](../../com.aspose.tasks/textstyle) 类的一个新实例。

### TextStyle(float fontSize, int fontStyle) {#TextStyle-float-int-}
```
public TextStyle(float fontSize, int fontStyle)
```


使用默认字体以及指定的字体大小和样式初始化 [TextStyle](../../com.aspose.tasks/textstyle) 类的一个新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontSize | float | TextStyle 的字体大小。 |
| fontStyle | int | TextStyle 的字体样式。 |

### TextStyle(int fontStyle) {#TextStyle-int-}
```
public TextStyle(int fontStyle)
```


使用默认字体和指定的字体样式初始化 [TextStyle](../../com.aspose.tasks/textstyle) 类的一个新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontStyle | int | 要应用于默认字体的字体样式。 |

### TextStyle(FontDescriptor font) {#TextStyle-com.aspose.tasks.FontDescriptor-}
```
public TextStyle(FontDescriptor font)
```


使用指定的字体设置初始化 [TextStyle](../../com.aspose.tasks/textstyle) 类的一个新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | TextStyle 的字体。 |

### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


获取文本样式的背景颜色。`Color`([getBackgroundColor()](../../com.aspose.tasks/textstyle\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose.tasks/textstyle\#setBackgroundColor-java.awt.Color-)).

**Returns:**
java.awt.Color - 文本样式的背景颜色。
### getBackgroundPattern() {#getBackgroundPattern--}
```
public final int getBackgroundPattern()
```


获取文本样式的背景图案。`BackgroundPattern`([getBackgroundPattern()](../../com.aspose.tasks/textstyle\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose.tasks/textstyle\#setBackgroundPattern-int-)).

**Returns:**
int - 文本样式的背景图案。
### getColor() {#getColor--}
```
public final Color getColor()
```


获取文本的颜色。

**Returns:**
java.awt.Color - 文本的颜色。
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


获取文本样式的字体。

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - font of the text style.
### getItemType() {#getItemType--}
```
public int getItemType()
```


获取文本样式的 [TextItemType](../../com.aspose.tasks/textitemtype)。

**Returns:**
int - 文本样式的 [TextItemType](../../com.aspose/tasks/textitemtype)。
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


设置文本样式的背景颜色。 `Color`([getBackgroundColor()](../../com.aspose.tasks/textstyle\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose.tasks/textstyle\#setBackgroundColor-java.awt.Color-)).

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color | 文本样式的背景颜色。 |

### setBackgroundPattern(int value) {#setBackgroundPattern-int-}
```
public final void setBackgroundPattern(int value)
```


设置文本样式的背景图案。 `BackgroundPattern`([getBackgroundPattern()](../../com.aspose.tasks/textstyle\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose.tasks/textstyle\#setBackgroundPattern-int-)).

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 文本样式的背景图案。 |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public final void setColor(Color value)
```


设置文本的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color | 文本的颜色。 |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


设置文本样式的字体。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | 文本样式的字体。 |

### setItemType(int value) {#setItemType-int-}
```
public void setItemType(int value)
```


设置文本样式的 [TextItemType](../../com.aspose.tasks/textitemtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | int | 文本样式的 [TextItemType](../../com.aspose.tasks/textitemtype)。 |

