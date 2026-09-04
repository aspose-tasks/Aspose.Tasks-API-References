---
title: "TableTextStyle"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示视图表中的文本样式。"
type: docs
weight: 288
url: /zh/java/com.aspose.tasks/tabletextstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.TextStyle](../../com.aspose.tasks/textstyle)
```
public class TableTextStyle extends TextStyle
```

表示视图表中的文本样式。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TableTextStyle(int rowUid)](#TableTextStyle-int-) | 初始化 [TableTextStyle](../../com.aspose.tasks/tabletextstyle) 类的新实例。 |
| [TableTextStyle(int rowUid, FontDescriptor font)](#TableTextStyle-int-com.aspose.tasks.FontDescriptor-) | 使用指定的字体初始化 [TableTextStyle](../../com.aspose.tasks/tabletextstyle) 类的新实例。 |
| [TableTextStyle(int rowUid, float fontSize, int fontStyle)](#TableTextStyle-int-float-int-) | 使用指定的字体大小和字体样式初始化 [TableTextStyle](../../com.aspose.tasks/tabletextstyle) 类的新实例。 |
| [TableTextStyle(int rowUid, int fontStyle)](#TableTextStyle-int-int-) | 使用默认字体设置和指定的字体样式初始化 [TableTextStyle](../../com.aspose.tasks/tabletextstyle) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getField()](#getField--) | 获取样式要应用的字段。 |
| [getItemType()](#getItemType--) | 返回文本项类型。 |
| [getRowUid()](#getRowUid--) | 获取行的唯一标识符。 |
| [setField(int value)](#setField-int-) | 设置样式要应用的字段。 |
### TableTextStyle(int rowUid) {#TableTextStyle-int-}
```
public TableTextStyle(int rowUid)
```


初始化 [TableTextStyle](../../com.aspose.tasks/tabletextstyle) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowUid | int | 指定的行唯一标识符。 |

### TableTextStyle(int rowUid, FontDescriptor font) {#TableTextStyle-int-com.aspose.tasks.FontDescriptor-}
```
public TableTextStyle(int rowUid, FontDescriptor font)
```


使用指定的字体初始化 [TableTextStyle](../../com.aspose.tasks/tabletextstyle) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowUid | int | 指定的行唯一标识符。 |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | 文本样式所基于的字体。 |

### TableTextStyle(int rowUid, float fontSize, int fontStyle) {#TableTextStyle-int-float-int-}
```
public TableTextStyle(int rowUid, float fontSize, int fontStyle)
```


使用指定的字体大小和字体样式初始化 [TableTextStyle](../../com.aspose.tasks/tabletextstyle) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowUid | int | 指定的行唯一标识符。 |
| fontSize | float | 文本样式所基于的字体大小。 |
| fontStyle | int | 字体样式。 |

### TableTextStyle(int rowUid, int fontStyle) {#TableTextStyle-int-int-}
```
public TableTextStyle(int rowUid, int fontStyle)
```


使用默认字体设置和指定的字体样式初始化 [TableTextStyle](../../com.aspose.tasks/tabletextstyle) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowUid | int | 指定的行唯一标识符。 |
| fontStyle | int | 字体样式。 |

### getField() {#getField--}
```
public final int getField()
```


获取样式要应用的字段。 `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Returns:**
int - 要应用样式的字段。
### getItemType() {#getItemType--}
```
public int getItemType()
```


返回文本项类型。

**Returns:**
int - TextItemType 枚举类型值。
### getRowUid() {#getRowUid--}
```
public final int getRowUid()
```


获取行的唯一标识符。

--------------------

如果样式要应用于视图的所有行，则返回 -1。

**Returns:**
int - 行的唯一标识符。
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


设置样式要应用的字段。 `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 要应用样式的字段。 |

