---
title: TimephasedData
second_title: Aspose.Tasks for Java API Reference
description: Represents a time phased data.
type: docs
weight: 319
url: /java/com.aspose.tasks/timephaseddata/
---

**Inheritance:**
java.lang.Object
```
public class TimephasedData
```

Represents a time phased data.
## Constructors

| Constructor | Description |
| --- | --- |
| [TimephasedData()](#TimephasedData--) | Initializes a new instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class. |
## Methods

| Method | Description |
| --- | --- |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-) | Creates and initializes a new instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data. |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Creates and initializes a new instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data. |
| [createUnitTimephased(int uid, Date start, Date finish, double units, byte type)](#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-) | Creates and initializes a new instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for unit-based time phased data of an assignment of a material resource. |
| [createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Creates and initializes a new instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data. |
| [getFinish()](#getFinish--) | Gets the finish date of a time phased data period. |
| [getStart()](#getStart--) | Gets the start date of a time phased data period. |
| [getTimephasedDataType()](#getTimephasedDataType--) | Gets the type of a time phased data. |
| [getUid()](#getUid--) | Gets the unique identifier of a time phased data |
| [getUnit()](#getUnit--) | Gets the time unit of a time phased data period. |
| [getValue()](#getValue--) | Gets the value per unit of time for a time phased data period. |
| [getValueToCost()](#getValueToCost--) | Gets `double` instance which represents string value of this object. |
| [getValueToDuration()](#getValueToDuration--) | Gets double instance which represents string value of this object. |
| [getValueToUnits()](#getValueToUnits--) | Gets `double` instance which represents string value of this object for unit-based time phased data. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Sets the finish date of a time phased data period. |
| [setStart(Date value)](#setStart-java.util.Date-) | Sets the start date of a time phased data period. |
| [setTimephasedDataType(byte value)](#setTimephasedDataType-byte-) | Sets the type of a time phased data. |
| [setUid(int value)](#setUid-int-) | Sets the unique identifier of a time phased data |
| [setUnit(byte value)](#setUnit-byte-) | Sets the time unit of a time phased data period. |
| [setValue(String value)](#setValue-java.lang.String-) | Sets the value per unit of time for a time phased data period. |
| [setValueToCost(double value)](#setValueToCost-double-) | `double` instance which represents string value of this object. |
### TimephasedData() {#TimephasedData--}
```
public TimephasedData()
```


Initializes a new instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class.

### createCostTimephased(int uid, Date start, Date finish, double value, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte type)
```


Creates and initializes a new instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | int | UID of the task. |
| start | java.util.Date | start date-time. |
| finish | java.util.Date | Finish date-time. |
| value | double | Cost value. |
| type | byte | Time-phased data type. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Creates and initializes a new instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | int | UID of the task. |
| start | java.util.Date | start date-time. |
| finish | java.util.Date | Finish date-time. |
| value | double | Cost value. |
| timeUnit | byte | Time unit type. |
| type | byte | Time-phased data type. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createUnitTimephased(int uid, Date start, Date finish, double units, byte type) {#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createUnitTimephased(int uid, Date start, Date finish, double units, byte type)
```


Creates and initializes a new instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for unit-based time phased data of an assignment of a material resource.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | int | UID of the task. |
| start | java.util.Date | Start date-time. |
| finish | java.util.Date | Finish date-time. |
| units | double | Number of units. |
| type | byte | Time-phased data type. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Creates and initializes a new instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | int | UID of the task. |
| start | java.util.Date | start date-time. |
| finish | java.util.Date | Finish date-time. |
| value | double | Timespan value. |
| timeUnit | byte | Time unit type. |
| type | byte | Time-phased data type. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Gets the finish date of a time phased data period.

**Returns:**
java.util.Date - the finish date of a time phased data period.
### getStart() {#getStart--}
```
public final Date getStart()
```


Gets the start date of a time phased data period.

**Returns:**
java.util.Date - the start date of a time phased data period.
### getTimephasedDataType() {#getTimephasedDataType--}
```
public final byte getTimephasedDataType()
```


Gets the type of a time phased data.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) property will be cleared, if it is not suitable for type, specified here.

**Returns:**
byte - the type of a time phased data.
### getUid() {#getUid--}
```
public final int getUid()
```


Gets the unique identifier of a time phased data

**Returns:**
int - the unique identifier of a time phased data
### getUnit() {#getUnit--}
```
public final byte getUnit()
```


Gets the time unit of a time phased data period.

**Returns:**
byte - the time unit of a time phased data period.
### getValue() {#getValue--}
```
public final String getValue()
```


Gets the value per unit of time for a time phased data period.

**Returns:**
java.lang.String - the value per unit of time for a time phased data period.
### getValueToCost() {#getValueToCost--}
```
public final double getValueToCost()
```


Gets `double` instance which represents string value of this object.

**Returns:**
double - a floating point representation of the object.
### getValueToDuration() {#getValueToDuration--}
```
public final double getValueToDuration()
```


Gets double instance which represents string value of this object.

**Returns:**
double - a time span representation of the object.
### getValueToUnits() {#getValueToUnits--}
```
public final double getValueToUnits()
```


Gets `double` instance which represents string value of this object for unit-based time phased data.

**Returns:**
double - a floating point representation of this object.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Sets the finish date of a time phased data period.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | the finish date of a time phased data period. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Sets the start date of a time phased data period.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | the start date of a time phased data period. |

### setTimephasedDataType(byte value) {#setTimephasedDataType-byte-}
```
public final void setTimephasedDataType(byte value)
```


Sets the type of a time phased data.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) property will be cleared, if it is not suitable for type, specified here.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | the type of a time phased data. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Sets the unique identifier of a time phased data

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the unique identifier of a time phased data |

### setUnit(byte value) {#setUnit-byte-}
```
public final void setUnit(byte value)
```


Sets the time unit of a time phased data period.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | the time unit of a time phased data period. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Sets the value per unit of time for a time phased data period.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the value per unit of time for a time phased data period. |

### setValueToCost(double value) {#setValueToCost-double-}
```
public final void setValueToCost(double value)
```


`double` instance which represents string value of this object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | `double` instance which represents string value of this object. |

