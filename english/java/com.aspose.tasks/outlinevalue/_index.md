---
title: OutlineValue
second_title: Aspose.Tasks for Java API Reference
description: Represents an outline value.
type: docs
weight: 162
url: /java/com.aspose.tasks/outlinevalue/
---

**Inheritance:**
java.lang.Object
```
public class OutlineValue
```

Represents an outline value.
## Constructors

| Constructor | Description |
| --- | --- |
| [OutlineValue()](#OutlineValue--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getDescription()](#getDescription--) | Gets the description of an outline value. |
| [getDurationValue()](#getDurationValue--) | Gets the duration if Type is Duration. |
| [getParentValueId()](#getParentValueId--) | Gets the Id of a parent node of an outline code. |
| [getType()](#getType--) | Gets the outline code type. |
| [getValue()](#getValue--) | Gets the actual value. |
| [getValueGuid()](#getValueGuid--) | Gets a GUID which identifies this value among others in the entire project. |
| [getValueId()](#getValueId--) | Gets the unique Id of an outline code value within a project. |
| [isCollapsed()](#isCollapsed--) | Gets a value indicating whether outline value is collapsed or not. |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | Sets a value indicating whether outline value is collapsed or not. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Sets the description of an outline value. |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Sets the duration if Type is Duration. |
| [setParentValueId(int value)](#setParentValueId-int-) | Sets the Id of a parent node of an outline code. |
| [setType(int value)](#setType-int-) | Sets the outline code type. |
| [setValue(String value)](#setValue-java.lang.String-) | Sets the actual value. |
| [setValueId(int value)](#setValueId-int-) | Sets the unique Id of an outline code value within a project. |
### OutlineValue() {#OutlineValue--}
```
public OutlineValue()
```


### getDescription() {#getDescription--}
```
public final String getDescription()
```


Gets the description of an outline value.

**Returns:**
java.lang.String - the description of an outline value.
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Gets the duration if Type is Duration.

--------------------

Prefer this property over the  Value ([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), when you need to set the value for OutlineValues with Duration type .

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration if Type is Duration.
### getParentValueId() {#getParentValueId--}
```
public final int getParentValueId()
```


Gets the Id of a parent node of an outline code.

**Returns:**
int - the Id of a parent node of an outline code.
### getType() {#getType--}
```
public final int getType()
```


Gets the outline code type.

**Returns:**
int - the outline code type.
### getValue() {#getValue--}
```
public final String getValue()
```


Gets the actual value.

**Returns:**
java.lang.String - the actual value.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Gets a GUID which identifies this value among others in the entire project.

**Returns:**
java.util.UUID - a GUID which identifies this value among others in the entire project.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Gets the unique Id of an outline code value within a project.

**Returns:**
int - the unique Id of an outline code value within a project.
### isCollapsed() {#isCollapsed--}
```
public final boolean isCollapsed()
```


Gets a value indicating whether outline value is collapsed or not.

--------------------

This is new for MS Project 2010 property.

**Returns:**
boolean - a value indicating whether outline value is collapsed or not.
### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public final void setCollapsed(boolean value)
```


Sets a value indicating whether outline value is collapsed or not.

--------------------

This is new for MS Project 2010 property.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether outline value is collapsed or not. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Sets the description of an outline value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the description of an outline value. |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Sets the duration if Type is Duration.

--------------------

Prefer this property over the  Value ([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), when you need to set the value for OutlineValues with Duration type .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | the duration if Type is Duration. |

### setParentValueId(int value) {#setParentValueId-int-}
```
public final void setParentValueId(int value)
```


Sets the Id of a parent node of an outline code.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the Id of a parent node of an outline code. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Sets the outline code type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the outline code type. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Sets the actual value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the actual value. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Sets the unique Id of an outline code value within a project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the unique Id of an outline code value within a project. |

