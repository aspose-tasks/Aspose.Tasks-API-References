---
title: GroupCriterion
second_title: Aspose.Tasks for Java API Reference
description: Represents a criterion in a group definition.
type: docs
weight: 119
url: /java/com.aspose.tasks/groupcriterion/
---

**Inheritance:**
java.lang.Object
```
public class GroupCriterion
```

Represents a criterion in a group definition. The GroupCriterion object is a member of the [GroupCriterionCollection](../../com.aspose.tasks/groupcriterioncollection) collection.
## Constructors

| Constructor | Description |
| --- | --- |
| [GroupCriterion()](#GroupCriterion--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [getAscending()](#getAscending--) | Gets a value indicating whether a field used as a criterion in a group definition is sorted in ascending order. |
| [getCellColor()](#getCellColor--) | Gets the color of the cell background for a field used as a criterion in a group definition. |
| [getField()](#getField--) | Gets the field being grouped by. |
| [getFont()](#getFont--) | Gets the font for a criterion in a group definition. |
| [getFontColor()](#getFontColor--) | Gets the color of the font for a field used as a criterion in a group definition. |
| [getGroupInterval()](#getGroupInterval--) | Gets the interval for a field used as a criterion in a group definition. |
| [getGroupOn()](#getGroupOn--) | Gets the type of grouping for a field used as a criterion in a group definition. |
| [getIndex()](#getIndex--) | Gets the index of a [GroupCriterion](../../com.aspose.tasks/groupcriterion) object in the containing [GroupCriterionCollection](../../com.aspose.tasks/groupcriterioncollection) collection. |
| [getParentGroup()](#getParentGroup--) | Gets the parent of the [GroupCriterion](../../com.aspose.tasks/groupcriterion) object. |
| [getPattern()](#getPattern--) | Gets the pattern of the cell for a field used as a criterion in a group definition. |
| [getStartAt()](#getStartAt--) | Gets the start of the intervals for a field used as a criterion in a group definition. |
| [hashCode()](#hashCode--) | Serves as a hash function for a particular type. |
| [setAscending(boolean value)](#setAscending-boolean-) | Sets a value indicating whether a field used as a criterion in a group definition is sorted in ascending order. |
| [setCellColor(Color value)](#setCellColor-java.awt.Color-) | Sets the color of the cell background for a field used as a criterion in a group definition. |
| [setField(int value)](#setField-int-) | Sets the field being grouped by. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | Sets the font for a criterion in a group definition. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Sets the color of the font for a field used as a criterion in a group definition. |
| [setGroupInterval(Object value)](#setGroupInterval-java.lang.Object-) | Sets the interval for a field used as a criterion in a group definition. |
| [setGroupOn(int value)](#setGroupOn-int-) | Sets the type of grouping for a field used as a criterion in a group definition. |
| [setPattern(int value)](#setPattern-int-) | Sets the pattern of the cell for a field used as a criterion in a group definition. |
| [setStartAt(Object value)](#setStartAt-java.lang.Object-) | Sets the start of the intervals for a field used as a criterion in a group definition. |
### GroupCriterion() {#GroupCriterion--}
```
public GroupCriterion()
```


### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returns a value indicating whether this instance is equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The object to compare with this instance. |

**Returns:**
boolean - **True** if o is a GroupCriterion that has the same UID value as this instance; otherwise, **false**.
### getAscending() {#getAscending--}
```
public final boolean getAscending()
```


Gets a value indicating whether a field used as a criterion in a group definition is sorted in ascending order. False if the field is sorted in descending order.

**Returns:**
boolean - a value indicating whether a field used as a criterion in a group definition is sorted in ascending order.
### getCellColor() {#getCellColor--}
```
public final Color getCellColor()
```


Gets the color of the cell background for a field used as a criterion in a group definition.

**Returns:**
java.awt.Color - the color of the cell background for a field used as a criterion in a group definition.
### getField() {#getField--}
```
public final int getField()
```


Gets the field being grouped by.

**Returns:**
int - the field being grouped by.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


Gets the font for a criterion in a group definition.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font for a criterion in a group definition.
### getFontColor() {#getFontColor--}
```
public final Color getFontColor()
```


Gets the color of the font for a field used as a criterion in a group definition.

**Returns:**
java.awt.Color - the color of the font for a field used as a criterion in a group definition.
### getGroupInterval() {#getGroupInterval--}
```
public final Object getGroupInterval()
```


Gets the interval for a field used as a criterion in a group definition.

**Returns:**
java.lang.Object - the interval for a field used as a criterion in a group definition.
### getGroupOn() {#getGroupOn--}
```
public final int getGroupOn()
```


Gets the type of grouping for a field used as a criterion in a group definition.

**Returns:**
int - the type of grouping for a field used as a criterion in a group definition.
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Gets the index of a [GroupCriterion](../../com.aspose.tasks/groupcriterion) object in the containing [GroupCriterionCollection](../../com.aspose.tasks/groupcriterioncollection) collection.

**Returns:**
int - the index of a [GroupCriterion](../../com.aspose.tasks/groupcriterion) object in the containing [GroupCriterionCollection](../../com.aspose.tasks/groupcriterioncollection) collection.
### getParentGroup() {#getParentGroup--}
```
public final Group getParentGroup()
```


Gets the parent of the [GroupCriterion](../../com.aspose.tasks/groupcriterion) object.

**Returns:**
[Group](../../com.aspose.tasks/group) - the parent of the [GroupCriterion](../../com.aspose.tasks/groupcriterion) object.
### getPattern() {#getPattern--}
```
public final int getPattern()
```


Gets the pattern of the cell for a field used as a criterion in a group definition.

**Returns:**
int - the pattern of the cell for a field used as a criterion in a group definition.
### getStartAt() {#getStartAt--}
```
public final Object getStartAt()
```


Gets the start of the intervals for a field used as a criterion in a group definition.

**Returns:**
java.lang.Object - the start of the intervals for a field used as a criterion in a group definition.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Serves as a hash function for a particular type.

**Returns:**
int - A hash code for the current Object.
### setAscending(boolean value) {#setAscending-boolean-}
```
public final void setAscending(boolean value)
```


Sets a value indicating whether a field used as a criterion in a group definition is sorted in ascending order. False if the field is sorted in descending order.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether a field used as a criterion in a group definition is sorted in ascending order. |

### setCellColor(Color value) {#setCellColor-java.awt.Color-}
```
public final void setCellColor(Color value)
```


Sets the color of the cell background for a field used as a criterion in a group definition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color | the color of the cell background for a field used as a criterion in a group definition. |

### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Sets the field being grouped by.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the field being grouped by. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


Sets the font for a criterion in a group definition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | the font for a criterion in a group definition. |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public final void setFontColor(Color value)
```


Sets the color of the font for a field used as a criterion in a group definition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color | the color of the font for a field used as a criterion in a group definition. |

### setGroupInterval(Object value) {#setGroupInterval-java.lang.Object-}
```
public final void setGroupInterval(Object value)
```


Sets the interval for a field used as a criterion in a group definition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object | the interval for a field used as a criterion in a group definition. |

### setGroupOn(int value) {#setGroupOn-int-}
```
public final void setGroupOn(int value)
```


Sets the type of grouping for a field used as a criterion in a group definition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the type of grouping for a field used as a criterion in a group definition. |

### setPattern(int value) {#setPattern-int-}
```
public final void setPattern(int value)
```


Sets the pattern of the cell for a field used as a criterion in a group definition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the pattern of the cell for a field used as a criterion in a group definition. |

### setStartAt(Object value) {#setStartAt-java.lang.Object-}
```
public final void setStartAt(Object value)
```


Sets the start of the intervals for a field used as a criterion in a group definition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object | the start of the intervals for a field used as a criterion in a group definition. |

