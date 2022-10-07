---
title: ExtendedAttribute
second_title: Aspose.Tasks for Java API Reference
description: Represents extended attributes.
type: docs
weight: 81
url: /java/com.aspose.tasks/extendedattribute/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttribute
```

Represents extended attributes.

--------------------

Currently supported all types of Extended attributes reading from MSP Xml 2003/2007 and mpp 2003. For MSP mpp 2007 all Extended attributes reading supported except durations and flags.
## Methods

| Method | Description |
| --- | --- |
| [getAttributeDefinition()](#getAttributeDefinition--) | Gets the attribute definition. |
| [getDateValue()](#getDateValue--) | Gets a value for attributes with date types (Date, Start, Finish). |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Sets a value for attributes with date types (Date, Start, Finish). |
| [getDurationValue()](#getDurationValue--) | Gets value for attributes with 'Duration' type. |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Sets value for attributes with 'Duration' type. |
| [getFieldId()](#getFieldId--) | Gets the id of a field. |
| [getFlagValue()](#getFlagValue--) | Gets a value indicating whether a flag is set for an attribute with 'Flag' type. |
| [setFlagValue(boolean value)](#setFlagValue-boolean-) | Sets a value indicating whether a flag is set for an attribute with 'Flag' type. |
| [getNumericValue()](#getNumericValue--) | Gets a value for attributes with numeric types (Cost, Number). |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Sets a value for attributes with numeric types (Cost, Number). |
| [getTextValue()](#getTextValue--) | Gets a value for attributes with 'Text' type. |
| [setTextValue(String value)](#setTextValue-java.lang.String-) | Sets a value for attributes with 'Text' type. |
| [getValueGuid()](#getValueGuid--) | Gets the guid of a lookup value. |
| [getValueReadOnly()](#getValueReadOnly--) | Gets a value indicating whether a value of this [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) instance is read-only. |
| [isErrorValue()](#isErrorValue--) | Gets whether calculation of extended attribute's value resulted in an error. |
| [toString()](#toString--) | Returns short string representation of an extended attribute. |
### getAttributeDefinition() {#getAttributeDefinition--}
```
public final ExtendedAttributeDefinition getAttributeDefinition()
```


Gets the attribute definition.

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the attribute definition.
### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Gets a value for attributes with date types (Date, Start, Finish).

**Returns:**
java.util.Date - a value for attributes with date types (Date, Start, Finish).
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Sets a value for attributes with date types (Date, Start, Finish).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value for attributes with date types (Date, Start, Finish). |

### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Gets value for attributes with 'Duration' type.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - value for attributes with 'Duration' type.
### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Sets value for attributes with 'Duration' type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | value for attributes with 'Duration' type. |

### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Gets the id of a field.

**Returns:**
java.lang.String - the id of a field.
### getFlagValue() {#getFlagValue--}
```
public final boolean getFlagValue()
```


Gets a value indicating whether a flag is set for an attribute with 'Flag' type.

**Returns:**
boolean - a value indicating whether a flag is set for an attribute with 'Flag' type.
### setFlagValue(boolean value) {#setFlagValue-boolean-}
```
public final void setFlagValue(boolean value)
```


Sets a value indicating whether a flag is set for an attribute with 'Flag' type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether a flag is set for an attribute with 'Flag' type. |

### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Gets a value for attributes with numeric types (Cost, Number).

**Returns:**
java.math.BigDecimal - a value for attributes with numeric types (Cost, Number).
### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Sets a value for attributes with numeric types (Cost, Number).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value for attributes with numeric types (Cost, Number). |

### getTextValue() {#getTextValue--}
```
public final String getTextValue()
```


Gets a value for attributes with 'Text' type.

**Returns:**
java.lang.String - a value for attributes with 'Text' type.
### setTextValue(String value) {#setTextValue-java.lang.String-}
```
public final void setTextValue(String value)
```


Sets a value for attributes with 'Text' type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value for attributes with 'Text' type. |

### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Gets the guid of a lookup value.

--------------------

Should not be set directly, instead use ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) to create an extended attribute with a lookup value.

**Returns:**
java.lang.String - the guid of a lookup value.
### getValueReadOnly() {#getValueReadOnly--}
```
public final boolean getValueReadOnly()
```


Gets a value indicating whether a value of this [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) instance is read-only.

Value: returns true if a formula or rollup is defined in the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) for this object.

**Returns:**
boolean - a value indicating whether a value of this [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) instance is read-only.
### isErrorValue() {#isErrorValue--}
```
public final boolean isErrorValue()
```


Gets whether calculation of extended attribute's value resulted in an error.

**Returns:**
boolean - whether calculation of extended attribute's value resulted in an error.
### toString() {#toString--}
```
public String toString()
```


Returns short string representation of an extended attribute.

**Returns:**
java.lang.String - The string representation of the extended attribute.
