---
title: "VisualObjectPlacement"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示在视图中 的放置和外观。"
type: docs
weight: 346
url: /zh/java/com.aspose.tasks/visualobjectplacement/
---

**Inheritance:**
java.lang.Object
```
public final class VisualObjectPlacement
```

表示在视图中 [OleObject](../../com.aspose/tasks/oleobject) 的放置和外观。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [VisualObjectPlacement()](#VisualObjectPlacement--) | 初始化 [VisualObjectPlacement](../../com.aspose/tasks/visualobjectplacement) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getAttachmentPoint()](#getAttachmentPoint--) | 当选择“Attach to task”选项时，获取视觉对象相对于任务的对齐方式。 |
| [getBorderLineColor()](#getBorderLineColor--) | 获取边框线颜色。 |
| [getBorderLineThickness()](#getBorderLineThickness--) | 获取边框线粗细（允许的值为 0 - 5）。 |
| [getFillColor()](#getFillColor--) | 获取填充颜色。 |
| [getFillPattern()](#getFillPattern--) | 获取填充图案。 |
| [getHeight()](#getHeight--) | 获取可视对象的显示高度。 |
| [getHorizontalOffset()](#getHorizontalOffset--) | 获取可视对象的水平偏移。 |
| [getOleObjectId()](#getOleObjectId--) | 获取 [OleObject](../../com.aspose.tasks/oleobject) 对象的 Id。 |
| [getTaskId()](#getTaskId--) | 如果选择了“附加到任务”选项，则获取任务的 Id，否则为 -1。 |
| [getTimescaleDate()](#getTimescaleDate--) | 当选择“附加到时间尺度”选项时，获取可视对象的日期放置位置。 |
| [getVerticalOffset()](#getVerticalOffset--) | 获取可视对象的垂直偏移。 |
| [getWidth()](#getWidth--) | 获取可视对象的显示宽度。 |
| [setAttachmentPoint(int value)](#setAttachmentPoint-int-) | 当选择“附加到任务”选项时，设置可视对象相对于任务的对齐方式。 |
| [setBorderLineColor(Color value)](#setBorderLineColor-java.awt.Color-) | 设置边框线颜色。 |
| [setBorderLineThickness(byte value)](#setBorderLineThickness-byte-) | 设置边框线粗细（允许的值为 0 - 5）。 |
| [setFillColor(Color value)](#setFillColor-java.awt.Color-) | 设置填充颜色。 |
| [setFillPattern(int value)](#setFillPattern-int-) | 设置填充图案。 |
| [setHeight(double value)](#setHeight-double-) | 设置可视对象的显示高度。 |
| [setHorizontalOffset(double value)](#setHorizontalOffset-double-) | 设置可视对象的水平偏移。 |
| [setOleObjectId(int value)](#setOleObjectId-int-) | 设置 [OleObject](../../com.aspose.tasks/oleobject) 对象的 Id。 |
| [setTaskId(int value)](#setTaskId-int-) | 如果选择了“附加到任务”选项，则设置任务的 Id，否则为 -1。 |
| [setTimescaleDate(Date value)](#setTimescaleDate-java.util.Date-) | 当选择“附加到时间尺度”选项时，设置可视对象的日期放置位置。 |
| [setVerticalOffset(double value)](#setVerticalOffset-double-) | 设置可视对象的垂直偏移。 |
| [setWidth(double value)](#setWidth-double-) | 设置可视对象的显示宽度。 |
### VisualObjectPlacement() {#VisualObjectPlacement--}
```
public VisualObjectPlacement()
```


初始化 [VisualObjectPlacement](../../com.aspose/tasks/visualobjectplacement) 类的新实例。

### getAttachmentPoint() {#getAttachmentPoint--}
```
public final int getAttachmentPoint()
```


当选择“Attach to task”选项时，获取视觉对象相对于任务的对齐方式。

**Returns:**
int - 当选择“附加到任务”选项时，可视对象相对于任务的对齐方式。
### getBorderLineColor() {#getBorderLineColor--}
```
public final Color getBorderLineColor()
```


获取边框线颜色。

**Returns:**
java.awt.Color - 边框线颜色。
### getBorderLineThickness() {#getBorderLineThickness--}
```
public final byte getBorderLineThickness()
```


获取边框线粗细（允许的值为 0 - 5）。

**Returns:**
byte - 边框线粗细（允许值为 0 - 5）。
### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


获取填充颜色。

**Returns:**
java.awt.Color - 填充颜色。
### getFillPattern() {#getFillPattern--}
```
public final int getFillPattern()
```


获取填充图案。

**Returns:**
int - 填充图案。
### getHeight() {#getHeight--}
```
public final double getHeight()
```


获取可视对象的显示高度。

**Returns:**
double - 可视对象的显示高度。
### getHorizontalOffset() {#getHorizontalOffset--}
```
public final double getHorizontalOffset()
```


获取可视对象的水平偏移。

**Returns:**
double - 可视对象的水平偏移。
### getOleObjectId() {#getOleObjectId--}
```
public final int getOleObjectId()
```


获取 [OleObject](../../com.aspose.tasks/oleobject) 对象的 Id。

**Returns:**
int - [OleObject](../../com.aspose/tasks/oleobject) 对象的 Id。
### getTaskId() {#getTaskId--}
```
public final int getTaskId()
```


如果选择了“附加到任务”选项，则获取任务的 Id，否则为 -1。

**Returns:**
int - 如果选择了 'Attach to task' 选项，则为任务的 Id，否则为 -1。
### getTimescaleDate() {#getTimescaleDate--}
```
public final Date getTimescaleDate()
```


当选择“附加到时间尺度”选项时，获取可视对象的日期放置位置。

**Returns:**
java.util.Date - 当选择 'Attach to timescale' 选项时，可视对象的日期放置位置。
### getVerticalOffset() {#getVerticalOffset--}
```
public final double getVerticalOffset()
```


获取可视对象的垂直偏移。

**Returns:**
double - 可视对象的垂直偏移。
### getWidth() {#getWidth--}
```
public final double getWidth()
```


获取可视对象的显示宽度。

**Returns:**
double - 可视对象的显示宽度。
### setAttachmentPoint(int value) {#setAttachmentPoint-int-}
```
public final void setAttachmentPoint(int value)
```


当选择“附加到任务”选项时，设置可视对象相对于任务的对齐方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 当选择 'Attach to task' 选项时，可视对象相对于任务的对齐方式。 |

### setBorderLineColor(Color value) {#setBorderLineColor-java.awt.Color-}
```
public final void setBorderLineColor(Color value)
```


设置边框线颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color | 边框线颜色。 |

### setBorderLineThickness(byte value) {#setBorderLineThickness-byte-}
```
public final void setBorderLineThickness(byte value)
```


设置边框线粗细（允许的值为 0 - 5）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 字节 | 边框线粗细（允许值为 0 - 5）。 |

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


设置填充颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color | 填充颜色。 |

### setFillPattern(int value) {#setFillPattern-int-}
```
public final void setFillPattern(int value)
```


设置填充图案。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 填充图案。 |

### setHeight(double value) {#setHeight-double-}
```
public final void setHeight(double value)
```


设置可视对象的显示高度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 可视对象的显示高度。 |

### setHorizontalOffset(double value) {#setHorizontalOffset-double-}
```
public final void setHorizontalOffset(double value)
```


设置可视对象的水平偏移。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 可视对象的水平偏移。 |

### setOleObjectId(int value) {#setOleObjectId-int-}
```
public final void setOleObjectId(int value)
```


设置 [OleObject](../../com.aspose.tasks/oleobject) 对象的 Id。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | int | [OleObject](../../com.aspose/tasks/oleobject) 对象的 Id。 |

### setTaskId(int value) {#setTaskId-int-}
```
public final void setTaskId(int value)
```


如果选择了“附加到任务”选项，则设置任务的 Id，否则为 -1。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 如果选择了 'Attach to task' 选项，则为任务的 Id，否则为 -1。 |

### setTimescaleDate(Date value) {#setTimescaleDate-java.util.Date-}
```
public final void setTimescaleDate(Date value)
```


当选择“附加到时间尺度”选项时，设置可视对象的日期放置位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 当选择 'Attach to timescale' 选项时，可视对象的日期放置位置。 |

### setVerticalOffset(double value) {#setVerticalOffset-double-}
```
public final void setVerticalOffset(double value)
```


设置可视对象的垂直偏移。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 可视对象的垂直偏移。 |

### setWidth(double value) {#setWidth-double-}
```
public final void setWidth(double value)
```


设置可视对象的显示宽度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 可视对象的显示宽度。 |

