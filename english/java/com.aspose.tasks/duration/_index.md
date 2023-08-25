---
title: Duration
second_title: Aspose.Tasks for Java API Reference
description: Represents duration in a project.
type: docs
weight: 76
url: /java/com.aspose.tasks/duration/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Duration extends Struct<Duration> implements System.IEquatable<Duration>
```

Represents duration in a project.
## Constructors

| Constructor | Description |
| --- | --- |
| [Duration()](#Duration--) | Initializes a new instance of the [Duration](../../com.aspose.tasks/duration) struct with a specified TimeSpan value and TimeUnitType. |
## Methods

| Method | Description |
| --- | --- |
| [Clone()](#Clone--) | Creates and returns a deep copy of this instance. |
| [CloneTo(Duration that)](#CloneTo-com.aspose.tasks.Duration-) | Makes a deep copy of the instance into another instance. |
| [add(Duration d)](#add-com.aspose.tasks.Duration-) | Adds specified duration to this duration. |
| [add(double val)](#add-double-) | Adds specified double value to this duration. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [convert(byte timeUnitType)](#convert-byte-) | Converts Duration object to another duration with specified time units. |
| [equals(Duration other)](#equals-com.aspose.tasks.Duration-) | Returns a value indicating whether this instance is equal to a specified object. |
| [equals(Duration obj1, Duration obj2)](#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Returns a value indicating whether specified  obj1  instance is equal to the specified  obj2  instance. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [getTimeSpan()](#getTimeSpan--) | Gets  TimeSpan ([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) instance of this Duration object. |
| [getTimeUnit()](#getTimeUnit--) | Gets time unit type for this object. |
| [hashCode()](#hashCode--) | Returns a hash code value for this object. |
| [isElapsed()](#isElapsed--) | Gets a value indicating whether time unit is elapsed. |
| [isEstimated()](#isEstimated--) | Gets a value indicating whether time unit is estimated. |
| [op_Equality(Duration a, Duration b)](#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Returns a value indicating whether this instance is equal to a specified object. |
| [op_Inequality(Duration a, Duration b)](#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Returns a value indicating whether this instance is not equal to a specified object. |
| [parse(Project p, String value)](#parse-com.aspose.tasks.Project-java.lang.String-) | Converts the specified string to the instance of [Duration](../../com.aspose.tasks/duration) struct. |
| [parseTimeSpan(String value)](#parseTimeSpan-java.lang.String-) | Parses duration string in format "PT--H--M--S--". |
| [subtract(Duration d)](#subtract-com.aspose.tasks.Duration-) | Subtracts specified duration from this duration instance. |
| [subtract(double val)](#subtract-double-) | Subtracts specified double value from this duration instance. |
| [toDouble()](#toDouble--) | Converts Duration object to  double  value. |
| [toString()](#toString--) | Returns a string representation of this instance. |
### Duration() {#Duration--}
```
public Duration()
```


Initializes a new instance of the [Duration](../../com.aspose.tasks/duration) struct with a specified TimeSpan value and TimeUnitType.

### Clone() {#Clone--}
```
public Duration Clone()
```


Creates and returns a deep copy of this instance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a deep copy of this object.
### CloneTo(Duration that) {#CloneTo-com.aspose.tasks.Duration-}
```
public void CloneTo(Duration that)
```


Makes a deep copy of the instance into another instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| that | [Duration](../../com.aspose.tasks/duration) | another instance. |

### add(Duration d) {#add-com.aspose.tasks.Duration-}
```
public final Duration add(Duration d)
```


Adds specified duration to this duration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | specified [Duration](../../com.aspose.tasks/duration) to add to this instance. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### add(double val) {#add-double-}
```
public final Duration add(double val)
```


Adds specified double value to this duration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| val | double | the specified  double  value to add to this instance. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### convert(byte timeUnitType) {#convert-byte-}
```
public final Duration convert(byte timeUnitType)
```


Converts Duration object to another duration with specified time units.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| timeUnitType | byte | the specified time unit type. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - returns new duration with the specified unit type.
### equals(Duration other) {#equals-com.aspose.tasks.Duration-}
```
public final boolean equals(Duration other)
```


Returns a value indicating whether this instance is equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [Duration](../../com.aspose.tasks/duration) | The object to compare with this instance. |

**Returns:**
boolean - Returns **True** if other Duration instance has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.
### equals(Duration obj1, Duration obj2) {#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean equals(Duration obj1, Duration obj2)
```


Returns a value indicating whether specified  obj1  instance is equal to the specified  obj2  instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj1 | [Duration](../../com.aspose.tasks/duration) | the first object to compare. |
| obj2 | [Duration](../../com.aspose.tasks/duration) | the second object to compare. |

**Returns:**
boolean - returns true if specified  obj1  instance is equal to the specified  obj2  instance; otherwise, false.
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
boolean - **True** if the specified object is a Duration that has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.
### getTimeSpan() {#getTimeSpan--}
```
public final double getTimeSpan()
```


Gets  TimeSpan ([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) instance of this Duration object.

Value: The TimeSpan instance of this Duration object.

**Returns:**
double -  TimeSpan ([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) instance of this Duration object.
### getTimeUnit() {#getTimeUnit--}
```
public final byte getTimeUnit()
```


Gets time unit type for this object.

Value: The time unit type of this Duration instance.

**Returns:**
byte - time unit type for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code value for this object.

**Returns:**
int - returns a hash code value for this duration instance.
### isElapsed() {#isElapsed--}
```
public final boolean isElapsed()
```


Gets a value indicating whether time unit is elapsed.

Value: The flag which determines whether this Duration instance is elapsed.

**Returns:**
boolean - a value indicating whether time unit is elapsed.
### isEstimated() {#isEstimated--}
```
public final boolean isEstimated()
```


Gets a value indicating whether time unit is estimated.

Value: The flag which determines whether this Duration instance is estimated.

**Returns:**
boolean - a value indicating whether time unit is estimated.
### op_Equality(Duration a, Duration b) {#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Equality(Duration a, Duration b)
```


Returns a value indicating whether this instance is equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | The first duration. |
| b | [Duration](../../com.aspose.tasks/duration) | The second duration. |

**Returns:**
boolean - a value indicating whether this instance is equal to a specified object
### op_Inequality(Duration a, Duration b) {#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Inequality(Duration a, Duration b)
```


Returns a value indicating whether this instance is not equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | The first duration. |
| b | [Duration](../../com.aspose.tasks/duration) | The second duration. |

**Returns:**
boolean - a value indicating whether this instance is not equal to a specified object
### parse(Project p, String value) {#parse-com.aspose.tasks.Project-java.lang.String-}
```
public static Duration parse(Project p, String value)
```


Converts the specified string to the instance of [Duration](../../com.aspose.tasks/duration) struct.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| p | [Project](../../com.aspose.tasks/project) | the specified instance of [Project](../../com.aspose.tasks/project) class to convert duration for. |
| value | java.lang.String | the specified string to convert. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Returns the converted instance of [Duration](../../com.aspose.tasks/duration) struct.
### parseTimeSpan(String value) {#parseTimeSpan-java.lang.String-}
```
public static double parseTimeSpan(String value)
```


Parses duration string in format "PT--H--M--S--".

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the specified string to parse. |

**Returns:**
double - returns parsed instance of the  TimeSpan ([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) struct.
### subtract(Duration d) {#subtract-com.aspose.tasks.Duration-}
```
public final Duration subtract(Duration d)
```


Subtracts specified duration from this duration instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | the specified [Duration](../../com.aspose.tasks/duration) instance to subtract from this instance. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### subtract(double val) {#subtract-double-}
```
public final Duration subtract(double val)
```


Subtracts specified double value from this duration instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| val | double | specified  double  value to subtract from this instance. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### toDouble() {#toDouble--}
```
public final double toDouble()
```


Converts Duration object to  double  value.

**Returns:**
double - Converted value.
### toString() {#toString--}
```
public String toString()
```


Returns a string representation of this instance.

**Returns:**
java.lang.String - a string representation of this instance.
