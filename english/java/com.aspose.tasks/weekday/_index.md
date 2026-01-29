---
title: WeekDay
second_title: Aspose.Tasks for Java API Reference
description: Represents a weekday which either defines regular days of a week or exception days in a calendar.
type: docs
weight: 351
url: /java/com.aspose.tasks/weekday/
---

**Inheritance:**
java.lang.Object
```
public class WeekDay
```

Represents a weekday which either defines regular days of a week or exception days in a calendar.
## Constructors

| Constructor | Description |
| --- | --- |
| [WeekDay(int dayType)](#WeekDay-int-) | Initializes a new instance of the [WeekDay](../../com.aspose.tasks/weekday) class with the specified day type. |
| [WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes)](#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--) | Initializes a new instance of the [WeekDay](../../com.aspose.tasks/weekday) class with the specified day type and list of working time periods. |
| [WeekDay(int dayType, WorkingTime[] workingTimes)](#WeekDay-int-com.aspose.tasks.WorkingTime...-) | Initializes a new instance of the [WeekDay](../../com.aspose.tasks/weekday) class with the specified day type and working time periods. |
| [WeekDay()](#WeekDay--) | Initializes a new instance of the [WeekDay](../../com.aspose.tasks/weekday) class. |
## Methods

| Method | Description |
| --- | --- |
| [castToDayType(int dw)](#castToDayType-int-) | Casts .Net's [DayOfWeek](../../com.aspose.tasks/dayofweek) to `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)). |
| [createDefaultWorkingDay(int dayType)](#createDefaultWorkingDay-int-) | Creates default working day. |
| [deepClone()](#deepClone--) | Returns a deep copy of the week day. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [getDayType()](#getDayType--) | Gets the type of a day. |
| [getDayWorking()](#getDayWorking--) | Gets a value indicating whether the specified date or day type is working. |
| [getFromDate()](#getFromDate--) | Gets the beginning of an exception time. |
| [getToDate()](#getToDate--) | Gets the end of an exception time. |
| [getWorkingTime()](#getWorkingTime--) | Returns the working time for a week day. |
| [getWorkingTimes()](#getWorkingTimes--) | Gets WorkingTimeCollection for this WeekDay instance. |
| [hashCode()](#hashCode--) | Returns a hash code value for the instance of the [WeekDay](../../com.aspose.tasks/weekday) class. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Sets a value indicating whether the specified date or day type is working. |
| [setDefaultWorkingTime(WeekDay day)](#setDefaultWorkingTime-com.aspose.tasks.WeekDay-) | Sets default time periods for the specified week day. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Sets the beginning of an exception time. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Sets the end of an exception time. |
### WeekDay(int dayType) {#WeekDay-int-}
```
public WeekDay(int dayType)
```


Initializes a new instance of the [WeekDay](../../com.aspose.tasks/weekday) class with the specified day type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dayType | int | The specified day type. |

### WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes) {#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--}
```
public WeekDay(int dayType, List<WorkingTime> workingTimes)
```


Initializes a new instance of the [WeekDay](../../com.aspose.tasks/weekday) class with the specified day type and list of working time periods.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dayType | int | The specified day type. |
| workingTimes | java.util.List&lt;com.aspose.tasks.WorkingTime&gt; | List of working time periods. |

### WeekDay(int dayType, WorkingTime[] workingTimes) {#WeekDay-int-com.aspose.tasks.WorkingTime...-}
```
public WeekDay(int dayType, WorkingTime[] workingTimes)
```


Initializes a new instance of the [WeekDay](../../com.aspose.tasks/weekday) class with the specified day type and working time periods.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dayType | int | The specified day type. |
| workingTimes | [WorkingTime\[\]](../../com.aspose.tasks/workingtime) | Array of working time periods. |

### WeekDay() {#WeekDay--}
```
public WeekDay()
```


Initializes a new instance of the [WeekDay](../../com.aspose.tasks/weekday) class.

### castToDayType(int dw) {#castToDayType-int-}
```
public static int castToDayType(int dw)
```


Casts .Net's [DayOfWeek](../../com.aspose.tasks/dayofweek) to `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dw | int | The day of week to cast from. |

**Returns:**
int - A cast day type.
### createDefaultWorkingDay(int dayType) {#createDefaultWorkingDay-int-}
```
public static WeekDay createDefaultWorkingDay(int dayType)
```


Creates default working day.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dayType | int | The day type to create default working day from. |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - A default working day with working times 8-12 and 13-17.
### deepClone() {#deepClone--}
```
public final WeekDay deepClone()
```


Returns a deep copy of the week day.

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - Returns the deep copy of the week day.
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
boolean - **True** if the specified object is a WeekDay that has the same FromDate, ToDate values and WorkingTimes as this instance; otherwise, **false**.
### getDayType() {#getDayType--}
```
public final int getDayType()
```


Gets the type of a day.

**Returns:**
int - the type of a day.
### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Gets a value indicating whether the specified date or day type is working.

**Returns:**
boolean - a value indicating whether the specified date or day type is working.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Gets the beginning of an exception time.

**Returns:**
java.util.Date - the beginning of an exception time.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Gets the end of an exception time.

**Returns:**
java.util.Date - the end of an exception time.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Returns the working time for a week day.

**Returns:**
double - Working time.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Gets WorkingTimeCollection for this WeekDay instance. The collection of working times that define the time worked on the weekday.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - WorkingTimeCollection for this WeekDay instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code value for the instance of the [WeekDay](../../com.aspose.tasks/weekday) class.

**Returns:**
int - returns a hash code value for this object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Sets a value indicating whether the specified date or day type is working.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the specified date or day type is working. |

### setDefaultWorkingTime(WeekDay day) {#setDefaultWorkingTime-com.aspose.tasks.WeekDay-}
```
public static void setDefaultWorkingTime(WeekDay day)
```


Sets default time periods for the specified week day.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| day | [WeekDay](../../com.aspose.tasks/weekday) | The week day to set default working day on. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Sets the beginning of an exception time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | the beginning of an exception time. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Sets the end of an exception time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | the end of an exception time. |

