---
title: OutlineCode
second_title: Aspose.Tasks for Java API Reference
description: Represents a value of an outline code.
type: docs
weight: 155
url: /java/com.aspose.tasks/outlinecode/
---

**Inheritance:**
java.lang.Object
```
public class OutlineCode
```

Represents a value of an outline code.

--------------------

Two pieces of data are necessary - a pointer to the outline code table that is specified by the FieldId, and the value that is specified either by the ValueId or ValueGuid pointer to the value list.
## Constructors

| Constructor | Description |
| --- | --- |
| [OutlineCode()](#OutlineCode--) | Initializes a new instance of the [OutlineCode](../../com.aspose.tasks/outlinecode) class. |
| [OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)](#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-) | Initializes a new instance of the [OutlineCode](../../com.aspose.tasks/outlinecode) class using the specified Outline Code and one of its values. |
## Methods

| Method | Description |
| --- | --- |
| [getFieldId()](#getFieldId--) | Gets the number value of the project Id custom field. |
| [getValueGuid()](#getValueGuid--) | Gets the GUID of the value in the value list. |
| [getValueId()](#getValueId--) | Gets the Id in the value list associated with the definition in the outline code collection. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Sets the number value of the project Id custom field. |
| [setValueGuid(String value)](#setValueGuid-java.lang.String-) | Sets the GUID of the value in the value list. |
| [setValueId(int value)](#setValueId-int-) | Sets the Id in the value list associated with the definition in the outline code collection. |
### OutlineCode() {#OutlineCode--}
```
public OutlineCode()
```


Initializes a new instance of the [OutlineCode](../../com.aspose.tasks/outlinecode) class.

### OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue) {#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-}
```
public OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)
```


Initializes a new instance of the [OutlineCode](../../com.aspose.tasks/outlinecode) class using the specified Outline Code and one of its values.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| codeDefinition | [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) | outline code definition. |
| outlineValue | [OutlineValue](../../com.aspose.tasks/outlinevalue) | one of outline code definition values. |

### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Gets the number value of the project Id custom field.

**Returns:**
java.lang.String - the number value of the project Id custom field.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Gets the GUID of the value in the value list. The ValueGuid matches the FieldGuid in the value list.

**Returns:**
java.lang.String - the GUID of the value in the value list.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Gets the Id in the value list associated with the definition in the outline code collection.

**Returns:**
int - the Id in the value list associated with the definition in the outline code collection.
### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


Sets the number value of the project Id custom field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the number value of the project Id custom field. |

### setValueGuid(String value) {#setValueGuid-java.lang.String-}
```
public final void setValueGuid(String value)
```


Sets the GUID of the value in the value list. The ValueGuid matches the FieldGuid in the value list.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the GUID of the value in the value list. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Sets the Id in the value list associated with the definition in the outline code collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the Id in the value list associated with the definition in the outline code collection. |

