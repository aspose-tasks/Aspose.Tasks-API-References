---
title: Value
second_title: Aspose.Tasks for Java API Reference
description: Represents a value in a value list.
type: docs
weight: 330
url: /java/com.aspose.tasks/value/
---

**Inheritance:**
java.lang.Object
```
public class Value
```

Represents a value in a value list.
## Constructors

| Constructor | Description |
| --- | --- |
| [Value()](#Value--) | Initializes a new instance of the [Value](../../com.aspose.tasks/value) class. |
## Methods

| Method | Description |
| --- | --- |
| [getDateValue()](#getDateValue--) | Gets the actual value if it can be represented as DateTime. |
| [getDescription()](#getDescription--) | Gets the description of a value. |
| [getDuration()](#getDuration--) | Gets the actual value which is used to represent Duration. |
| [getId()](#getId--) | Gets the unique identifier of a value across a project. |
| [getNumericValue()](#getNumericValue--) | Gets the actual value which is used to represent number or cost value. |
| [getPhonetic()](#getPhonetic--) | Gets the phonetic information about custom field name. |
| [getStringValue()](#getStringValue--) | Gets the actual value which is used to represent Text string. |
| [getVal()](#getVal--) | Gets the actual value in internal representation. |
| [getValueGuid()](#getValueGuid--) | Gets a GUID which identifies this value among others in the entire project. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Sets the actual value if it can be represented as DateTime. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Sets the description of a value. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Sets the actual value which is used to represent Duration. |
| [setId(int value)](#setId-int-) | Sets the unique identifier of a value across a project. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Sets the actual value which is used to represent number or cost value. |
| [setPhonetic(String value)](#setPhonetic-java.lang.String-) | Sets the phonetic information about custom field name. |
| [setStringValue(String value)](#setStringValue-java.lang.String-) | Sets the actual value which is used to represent Text string. |
| [setVal(String value)](#setVal-java.lang.String-) | Sets the actual value in internal representation. |
### Value() {#Value--}
```
public Value()
```


Initializes a new instance of the [Value](../../com.aspose.tasks/value) class.

### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Gets the actual value if it can be represented as DateTime. Default value is DateTime\#MinValue.MinValue.

--------------------

Prefer this property over the `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), when you need to set the DateTime value.

**Returns:**
java.util.Date - the actual value if it can be represented as DateTime.
### getDescription() {#getDescription--}
```
public final String getDescription()
```


Gets the description of a value.

**Returns:**
java.lang.String - the description of a value.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Gets the actual value which is used to represent Duration.

--------------------

Prefer this property over the `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), when you need to set the Duration value.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the actual value which is used to represent Duration.
### getId() {#getId--}
```
public final int getId()
```


Gets the unique identifier of a value across a project.

It's important to not have same identifiers for different [Value](../../com.aspose.tasks/value) instances.

Minimal `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) value is `1`.

**Returns:**
int - the unique identifier of a value across a project.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Gets the actual value which is used to represent number or cost value.

--------------------

Prefer this property over the `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), when you need to set the Number or Cost value.

**Returns:**
java.math.BigDecimal - the actual value which is used to represent number or cost value.
### getPhonetic() {#getPhonetic--}
```
public final String getPhonetic()
```


Gets the phonetic information about custom field name.

**Returns:**
java.lang.String - the phonetic information about custom field name.
### getStringValue() {#getStringValue--}
```
public final String getStringValue()
```


Gets the actual value which is used to represent Text string.

--------------------

Prefer this property over the `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), when you need to set the Text value.

**Returns:**
java.lang.String - the actual value which is used to represent Text string.
### getVal() {#getVal--}
```
public final String getVal()
```


Gets the actual value in internal representation. Prefer using strongly typed properties which are listed below.

--------------------

If you want to set Text value prefer using strongly typed `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)) property.

If you want to set Number or Cost value prefer using strongly typed `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)) property.

If you want to set Date/Start/Finish values, prefer using strongly typed `DateValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) property.

If you want to set Duration value prefer using strongly typed `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)) property.

If your type wasn't listed, use `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) property.

**Returns:**
java.lang.String - the actual value in internal representation.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Gets a GUID which identifies this value among others in the entire project.

**Returns:**
java.util.UUID - a GUID which identifies this value among others in the entire project.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Sets the actual value if it can be represented as DateTime. Default value is DateTime\#MinValue.MinValue.

--------------------

Prefer this property over the `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), when you need to set the DateTime value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | the actual value if it can be represented as DateTime. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Sets the description of a value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the description of a value. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Sets the actual value which is used to represent Duration.

--------------------

Prefer this property over the `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), when you need to set the Duration value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | the actual value which is used to represent Duration. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Sets the unique identifier of a value across a project.

It's important to not have same identifiers for different [Value](../../com.aspose.tasks/value) instances.

Minimal `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) value is `1`.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the unique identifier of a value across a project. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Sets the actual value which is used to represent number or cost value.

--------------------

Prefer this property over the `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), when you need to set the Number or Cost value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | the actual value which is used to represent number or cost value. |

### setPhonetic(String value) {#setPhonetic-java.lang.String-}
```
public final void setPhonetic(String value)
```


Sets the phonetic information about custom field name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the phonetic information about custom field name. |

### setStringValue(String value) {#setStringValue-java.lang.String-}
```
public final void setStringValue(String value)
```


Sets the actual value which is used to represent Text string.

--------------------

Prefer this property over the `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), when you need to set the Text value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the actual value which is used to represent Text string. |

### setVal(String value) {#setVal-java.lang.String-}
```
public final void setVal(String value)
```


Sets the actual value in internal representation. Prefer using strongly typed properties which are listed below.

--------------------

If you want to set Text value prefer using strongly typed `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)) property.

If you want to set Number or Cost value prefer using strongly typed `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)) property.

If you want to set Date/Start/Finish values, prefer using strongly typed `DateTimeValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) property.

If you want to set Duration value prefer using strongly typed `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)) property.

If your type wasn't listed, use `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) property.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the actual value in internal representation. |

