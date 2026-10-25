---
title: "ViewColumn"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示项目视图中的列。"
type: docs
weight: 344
url: /zh/java/com.aspose.tasks/viewcolumn/
---

**Inheritance:**
java.lang.Object
```
public abstract class ViewColumn
```

表示项目视图中的列。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getField()](#getField--) | 获取列字段。 |
| [getName()](#getName--) | 获取列名。 |
| [getStringAlignment()](#getStringAlignment--) | 获取文本的对齐方式（可以是 [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) 枚举的其中一个值）。 |
| [getTextStyleModificationCallback()](#getTextStyleModificationCallback--) | 获取可用于自定义列单元格外观的回调。 |
| [getWidth()](#getWidth--) | 获取列宽度。 |
| [setField(int value)](#setField-int-) | 设置列字段。 |
| [setStringAlignment(int value)](#setStringAlignment-int-) | 设置文本的对齐方式（可以是 [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) 枚举的其中一个值）。 |
| [setTextStyleModificationCallback(ITextStyleModificationCallback value)](#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-) | 设置可用于自定义列单元格外观的回调。 |
### getField() {#getField--}
```
public abstract int getField()
```


获取列字段。`Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Returns:**
int - 列字段。
### getName() {#getName--}
```
public final String getName()
```


获取列名。

**Returns:**
java.lang.String - 列名。
### getStringAlignment() {#getStringAlignment--}
```
public final int getStringAlignment()
```


获取文本的对齐方式（可以是 [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) 枚举的其中一个值）。

**Returns:**
int - 文本的对齐方式（可以是 [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) 枚举的其中一个值）。
### getTextStyleModificationCallback() {#getTextStyleModificationCallback--}
```
public final ITextStyleModificationCallback getTextStyleModificationCallback()
```


获取可用于自定义列单元格外观的回调。

**Returns:**
[ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) - the callback which can be used to customize the appearance of the column's cells.
### getWidth() {#getWidth--}
```
public final int getWidth()
```


获取列宽度。

**Returns:**
int - 列宽度。
### setField(int value) {#setField-int-}
```
public abstract void setField(int value)
```


设置列字段。`Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 列字段。 |

### setStringAlignment(int value) {#setStringAlignment-int-}
```
public final void setStringAlignment(int value)
```


设置文本的对齐方式（可以是 [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) 枚举的其中一个值）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | int | 文本的对齐方式（可以是 [HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment) 枚举的其中一个值）。 |

### setTextStyleModificationCallback(ITextStyleModificationCallback value) {#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-}
```
public final void setTextStyleModificationCallback(ITextStyleModificationCallback value)
```


设置可用于自定义列单元格外观的回调。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) | 可用于自定义列单元格外观的回调。 |

