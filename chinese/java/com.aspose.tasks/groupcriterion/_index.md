---
title: "GroupCriterion"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示组定义中的一个准则。"
type: docs
weight: 124
url: /zh/java/com.aspose.tasks/groupcriterion/
---

**Inheritance:**
java.lang.Object
```
public class GroupCriterion
```

表示组定义中的一个准则。GroupCriterion 对象是 [GroupCriterionCollection](../../com.aspose.tasks/groupcriterioncollection) 集合的成员。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GroupCriterion()](#GroupCriterion--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [getAscending()](#getAscending--) | 获取一个值，指示在组定义中用作准则的字段是否按升序排序。 |
| [getCellColor()](#getCellColor--) | 获取在组定义中用作准则的字段的单元格背景颜色。 |
| [getField()](#getField--) | 获取用于分组的字段。 |
| [getFont()](#getFont--) | 获取组定义中准则的字体。 |
| [getFontColor()](#getFontColor--) | 获取在组定义中用作准则的字段的字体颜色。 |
| [getGroupInterval()](#getGroupInterval--) | 获取在组定义中用作准则的字段的间隔。 |
| [getGroupOn()](#getGroupOn--) | 获取在组定义中用作准则的字段的分组类型。 |
| [getPattern()](#getPattern--) | 获取在组定义中用作准则的字段的单元格模式。 |
| [getStartAt()](#getStartAt--) | 获取在组定义中用作准则的字段的间隔起始值。 |
| [hashCode()](#hashCode--) | 作为特定类型的哈希函数。 |
| [setAscending(boolean value)](#setAscending-boolean-) | 设置一个值，指示在组定义中用作准则的字段是否按升序排序。 |
| [setCellColor(Color value)](#setCellColor-java.awt.Color-) | 设置在组定义中用作准则的字段的单元格背景颜色。 |
| [setField(int value)](#setField-int-) | 设置用于分组的字段。 |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | 设置组定义中准则的字体。 |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | 设置在组定义中用作准则的字段的字体颜色。 |
| [setGroupInterval(Object value)](#setGroupInterval-java.lang.Object-) | 设置在组定义中用作准则的字段的间隔。 |
| [setGroupOn(int value)](#setGroupOn-int-) | 设置在组定义中用作准则的字段的分组类型。 |
| [setPattern(int value)](#setPattern-int-) | 设置在组定义中用作准则的字段的单元格模式。 |
| [setStartAt(Object value)](#setStartAt-java.lang.Object-) | 设置用于组定义中作为准则的字段的区间起始值。 |
### GroupCriterion() {#GroupCriterion--}
```
public GroupCriterion()
```


### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 用于与此实例比较的对象。 |

**Returns:**
boolean - 如果 o 是具有与此实例相同 UID 值的 GroupCriterion，则为 **True**；否则为 **false**。
### getAscending() {#getAscending--}
```
public final boolean getAscending()
```


获取一个值，指示用于组定义中作为准则的字段是否按升序排序。如果字段按降序排序，则为 False。

**Returns:**
boolean - 一个值，指示用于组定义中作为准则的字段是否按升序排序。
### getCellColor() {#getCellColor--}
```
public final Color getCellColor()
```


获取在组定义中用作准则的字段的单元格背景颜色。

**Returns:**
java.awt.Color - 用于组定义中作为准则的字段的单元格背景颜色。
### getField() {#getField--}
```
public final int getField()
```


获取用于分组的字段。

**Returns:**
int - 被分组的字段。
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


获取组定义中准则的字体。

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font for a criterion in a group definition.
### getFontColor() {#getFontColor--}
```
public final Color getFontColor()
```


获取在组定义中用作准则的字段的字体颜色。

**Returns:**
java.awt.Color - 用于组定义中作为准则的字段的字体颜色。
### getGroupInterval() {#getGroupInterval--}
```
public final Object getGroupInterval()
```


获取在组定义中用作准则的字段的间隔。

**Returns:**
java.lang.Object - 用于组定义中作为准则的字段的区间。
### getGroupOn() {#getGroupOn--}
```
public final int getGroupOn()
```


获取在组定义中用作准则的字段的分组类型。

**Returns:**
int - 用于组定义中作为准则的字段的分组类型。
### getPattern() {#getPattern--}
```
public final int getPattern()
```


获取在组定义中用作准则的字段的单元格模式。

**Returns:**
int - 用于组定义中作为准则的字段的单元格模式。
### getStartAt() {#getStartAt--}
```
public final Object getStartAt()
```


获取在组定义中用作准则的字段的间隔起始值。

**Returns:**
java.lang.Object - 用于组定义中作为准则的字段的区间起始值。
### hashCode() {#hashCode--}
```
public int hashCode()
```


作为特定类型的哈希函数。

**Returns:**
int - 当前 Object 的哈希码。
### setAscending(boolean value) {#setAscending-boolean-}
```
public final void setAscending(boolean value)
```


设置一个值，指示用于组定义中作为准则的字段是否按升序排序。如果字段按降序排序，则为 False。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示用于组定义中作为准则的字段是否按升序排序。 |

### setCellColor(Color value) {#setCellColor-java.awt.Color-}
```
public final void setCellColor(Color value)
```


设置在组定义中用作准则的字段的单元格背景颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color | 用于组定义中作为准则的字段的单元格背景颜色。 |

### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


设置用于分组的字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 被分组的字段。 |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


设置组定义中准则的字体。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | 组定义中准则的字体。 |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public final void setFontColor(Color value)
```


设置在组定义中用作准则的字段的字体颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color | 用于组定义中作为准则的字段的字体颜色。 |

### setGroupInterval(Object value) {#setGroupInterval-java.lang.Object-}
```
public final void setGroupInterval(Object value)
```


设置在组定义中用作准则的字段的间隔。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object | 用于组定义中作为准则的字段的区间。 |

### setGroupOn(int value) {#setGroupOn-int-}
```
public final void setGroupOn(int value)
```


设置在组定义中用作准则的字段的分组类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 用于组定义中作为准则的字段的分组类型。 |

### setPattern(int value) {#setPattern-int-}
```
public final void setPattern(int value)
```


设置在组定义中用作准则的字段的单元格模式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 用于组定义中作为准则的字段的单元格模式。 |

### setStartAt(Object value) {#setStartAt-java.lang.Object-}
```
public final void setStartAt(Object value)
```


设置用于组定义中作为准则的字段的区间起始值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object | 用于组定义中作为准则的字段的区间起始值。 |

