---
title: TimeDelta
second_title: Aspose.Tasks for Java API Reference
description: Represents a difference between two timestamps.
type: docs
weight: 314
url: /java/com.aspose.tasks/timedelta/
---

**Inheritance:**
java.lang.Object
```
public class TimeDelta
```

Represents a difference between two timestamps.
## Constructors

| Constructor | Description |
| --- | --- |
| [TimeDelta(int hours, int minutes, int seconds)](#TimeDelta-int-int-int-) | Initializes new instance of TimeDelta to the specified number of hours, minutes and seconds. |
| [TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)](#TimeDelta-int-int-int-int-int-) | Initializes new instance of TimeDelta to the specified number of days, hours, minutes, seconds and milliseconds. |
## Methods

| Method | Description |
| --- | --- |
| [add(TimeDelta other)](#add-com.aspose.tasks.TimeDelta-) | Returns a new TimeDelta object whose value is a sum of this and other instance. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [compare(TimeDelta t1, TimeDelta t2)](#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Compares two TimeDelta values and returns an integer that indicates whether the first value is shorter than, equal to, or longer than the second value. |
| [compareTo(TimeDelta other)](#compareTo-com.aspose.tasks.TimeDelta-) | Compares this instance to a specified TimeDelta object and returns an integer that indicates whether this instance is shorter than, equal to, or longer than the TimeSpan object. |
| [equals(TimeDelta other)](#equals-com.aspose.tasks.TimeDelta-) | Indicates whether some `other` time span is equal to this one. |
| [equals(TimeDelta t1, TimeDelta t2)](#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Checks two instances for equality. |
| [equals(Object other)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [fromDays(double value)](#fromDays-double-) | Returns a TimeDelta that represents a specified number of days (rounded to the nearest millisecond). |
| [fromHours(double value)](#fromHours-double-) | Returns a TimeDelta that represents a specified number of hours (rounded to the nearest millisecond). |
| [fromMilliseconds(double value)](#fromMilliseconds-double-) | Returns a TimeDelta that represents a specified number of milliseconds (rounded to the nearest millisecond). |
| [fromMinutes(double value)](#fromMinutes-double-) | Returns a TimeDelta that represents a specified number of minutes (rounded to the nearest millisecond). |
| [fromSeconds(double value)](#fromSeconds-double-) | Returns a TimeDelta that represents a specified number of seconds (rounded to the nearest millisecond). |
| [getDays()](#getDays--) | Returns the days component of the time interval, represented by this instance. |
| [getHours()](#getHours--) | Returns the hours component of the time interval, represented by this instance. |
| [getMilliseconds()](#getMilliseconds--) | Returns the milliseconds component of the time interval, represented by this instance. |
| [getMinutes()](#getMinutes--) | Returns the minutes component of the time interval, represented by this instance. |
| [getSeconds()](#getSeconds--) | Returns the seconds component of the time interval, represented by this instance. |
| [getTotalDays()](#getTotalDays--) | Returns the value of the current instance expressed in whole and fractional days. |
| [getTotalHours()](#getTotalHours--) | Returns the value of the current instance expressed in whole and fractional hours. |
| [getTotalMilliseconds()](#getTotalMilliseconds--) | Returns the value of the current instance expressed in whole and fractional milliseconds. |
| [getTotalMinutes()](#getTotalMinutes--) | Returns the value of the current instance expressed in whole and fractional minutes. |
| [getTotalSeconds()](#getTotalSeconds--) | Returns the value of the current instance expressed in whole and fractional seconds. |
| [hashCode()](#hashCode--) | \{@inheritDoc\} |
| [negate()](#negate--) | Returns a new `TimeDelta` whose value is the negated value of this instance. |
| [parse(String s)](#parse-java.lang.String-) | Converts the string representation of a time interval to its `TimeDelta` equivalent. |
| [subtract(TimeDelta other)](#subtract-com.aspose.tasks.TimeDelta-) | Returns a new TimeDelta object whose value is a difference between this and `other` instances. |
| [toString()](#toString--) | \{@inheritDoc\} |
| [tryParse(String s, TimeDelta[] result)](#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---) | Converts the string representation of a time interval to its TimeDelta equivalent and returns a value that indicates whether the conversion succeeded. |
### TimeDelta(int hours, int minutes, int seconds) {#TimeDelta-int-int-int-}
```
public TimeDelta(int hours, int minutes, int seconds)
```


Initializes new instance of TimeDelta to the specified number of hours, minutes and seconds.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| hours | int | number of hours. |
| minutes | int | number of minutes. |
| seconds | int | number of seconds. |

### TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds) {#TimeDelta-int-int-int-int-int-}
```
public TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)
```


Initializes new instance of TimeDelta to the specified number of days, hours, minutes, seconds and milliseconds.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| days | int | number of days. |
| hours | int | number of hours. |
| minutes | int | number of minutes. |
| seconds | int | number of seconds. |
| milliseconds | int | number of milliseconds. |

### add(TimeDelta other) {#add-com.aspose.tasks.TimeDelta-}
```
public TimeDelta add(TimeDelta other)
```


Returns a new TimeDelta object whose value is a sum of this and other instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | the instance to sum with. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance plus value of other instance.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### compare(TimeDelta t1, TimeDelta t2) {#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static int compare(TimeDelta t1, TimeDelta t2)
```


Compares two TimeDelta values and returns an integer that indicates whether the first value is shorter than, equal to, or longer than the second value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | the first time interval to compare. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | the second time interval to compare. |

**Returns:**
int - \-1 if `t1` is shorter than `t2`, 0 if `t1` equals to `t2` and 1 if `t1` is longer than `t2`.
### compareTo(TimeDelta other) {#compareTo-com.aspose.tasks.TimeDelta-}
```
public int compareTo(TimeDelta other)
```


Compares this instance to a specified TimeDelta object and returns an integer that indicates whether this instance is shorter than, equal to, or longer than the TimeSpan object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | an instance to compare with. |

**Returns:**
int - \-1 if this instance is shorter than `other`, 0 if this instance equals to `other` and 1 if this instance is longer than `other`.
### equals(TimeDelta other) {#equals-com.aspose.tasks.TimeDelta-}
```
public boolean equals(TimeDelta other)
```


Indicates whether some `other` time span is equal to this one.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | time span to compare with. |

**Returns:**
boolean - `true` if intervals equal; `false` otherwise.
### equals(TimeDelta t1, TimeDelta t2) {#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static boolean equals(TimeDelta t1, TimeDelta t2)
```


Checks two instances for equality.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | first instance. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | second instance. |

**Returns:**
boolean - `true` if instances are equal; `false` otherwise.
### equals(Object other) {#equals-java.lang.Object-}
```
public boolean equals(Object other)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### fromDays(double value) {#fromDays-double-}
```
public static TimeDelta fromDays(double value)
```


Returns a TimeDelta that represents a specified number of days (rounded to the nearest millisecond).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a number of days. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromHours(double value) {#fromHours-double-}
```
public static TimeDelta fromHours(double value)
```


Returns a TimeDelta that represents a specified number of hours (rounded to the nearest millisecond).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a number of hours. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMilliseconds(double value) {#fromMilliseconds-double-}
```
public static TimeDelta fromMilliseconds(double value)
```


Returns a TimeDelta that represents a specified number of milliseconds (rounded to the nearest millisecond).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a number of milliseconds. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMinutes(double value) {#fromMinutes-double-}
```
public static TimeDelta fromMinutes(double value)
```


Returns a TimeDelta that represents a specified number of minutes (rounded to the nearest millisecond).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a number of minutes. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromSeconds(double value) {#fromSeconds-double-}
```
public static TimeDelta fromSeconds(double value)
```


Returns a TimeDelta that represents a specified number of seconds (rounded to the nearest millisecond).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a number of seconds. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### getDays() {#getDays--}
```
public int getDays()
```


Returns the days component of the time interval, represented by this instance.

**Returns:**
int - the days component of the time inteval. Can be positive or negative.
### getHours() {#getHours--}
```
public int getHours()
```


Returns the hours component of the time interval, represented by this instance.

**Returns:**
int - the hours component of the time interval in range from -23 through 23.
### getMilliseconds() {#getMilliseconds--}
```
public int getMilliseconds()
```


Returns the milliseconds component of the time interval, represented by this instance.

**Returns:**
int - the milliseconds component of the time interval in range from -999 through 999.
### getMinutes() {#getMinutes--}
```
public int getMinutes()
```


Returns the minutes component of the time interval, represented by this instance.

**Returns:**
int - the minutes component of the time interval in range from -59 through 59.
### getSeconds() {#getSeconds--}
```
public int getSeconds()
```


Returns the seconds component of the time interval, represented by this instance.

**Returns:**
int - the seconds component of the time interval in range from -59 through 59.
### getTotalDays() {#getTotalDays--}
```
public double getTotalDays()
```


Returns the value of the current instance expressed in whole and fractional days.

**Returns:**
double - the total number of days represented by this instance.
### getTotalHours() {#getTotalHours--}
```
public double getTotalHours()
```


Returns the value of the current instance expressed in whole and fractional hours.

**Returns:**
double - the total number of hours represented by this instance.
### getTotalMilliseconds() {#getTotalMilliseconds--}
```
public double getTotalMilliseconds()
```


Returns the value of the current instance expressed in whole and fractional milliseconds.

**Returns:**
double - the total number of milliseconds represented by this instance.
### getTotalMinutes() {#getTotalMinutes--}
```
public double getTotalMinutes()
```


Returns the value of the current instance expressed in whole and fractional minutes.

**Returns:**
double - the total number of minutes represented by this instance.
### getTotalSeconds() {#getTotalSeconds--}
```
public double getTotalSeconds()
```


Returns the value of the current instance expressed in whole and fractional seconds.

**Returns:**
double - the total number of seconds represented by this instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int - \{@inheritDoc\}
### negate() {#negate--}
```
public TimeDelta negate()
```


Returns a new `TimeDelta` whose value is the negated value of this instance.

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - A new object with the same numeric value as this instance, but with the opposite sign.
### parse(String s) {#parse-java.lang.String-}
```
public static TimeDelta parse(String s)
```


Converts the string representation of a time interval to its `TimeDelta` equivalent.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| s | java.lang.String | a string that specifies the time interval to convert. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a time interval that corresponds to `s`.
### subtract(TimeDelta other) {#subtract-com.aspose.tasks.TimeDelta-}
```
public TimeDelta subtract(TimeDelta other)
```


Returns a new TimeDelta object whose value is a difference between this and `other` instances.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | the instance to subtract. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance minus value of other instance.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String - \{@inheritDoc\}
### tryParse(String s, TimeDelta[] result) {#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---}
```
public static boolean tryParse(String s, TimeDelta[] result)
```


Converts the string representation of a time interval to its TimeDelta equivalent and returns a value that indicates whether the conversion succeeded.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| s | java.lang.String | a string that specifies the time interval to convert. |
| result | [TimeDelta\[\]](../../com.aspose.tasks/timedelta) | this array must have at least one element. When this method returns, `result[0]` contains an object that represents the time interval specified by `s`, or a zero-length time interval if the conversion failed. |

**Returns:**
boolean - `true` if s was converted successfully; otherwise, `false`.
