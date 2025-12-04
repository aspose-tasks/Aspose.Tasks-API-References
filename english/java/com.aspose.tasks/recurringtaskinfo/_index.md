---
title: RecurringTaskInfo
second_title: Aspose.Tasks for Java API Reference
description: Represents the details of a recurring task in a project.
type: docs
weight: 243
url: /java/com.aspose.tasks/recurringtaskinfo/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskInfo
```

Represents the details of a recurring task in a project.
## Methods

| Method | Description |
| --- | --- |
| [getDailyRepetitions()](#getDailyRepetitions--) | Gets a number of repetitions for the daily recurrence pattern. |
| [getDailyUseWorkdays()](#getDailyUseWorkdays--) | Gets a value indicating whether to use workdays for the daily recurrence pattern. |
| [getDuration()](#getDuration--) | Gets the duration for one occurrence of the recurring task. |
| [getEndDate()](#getEndDate--) | Gets the date for the occurrences to end. |
| [getMonthlyDay()](#getMonthlyDay--) | Gets a number of day of the monthly recurrence pattern. |
| [getMonthlyOrdinalDay()](#getMonthlyOrdinalDay--) | Gets a day of the monthly recurrence pattern when using ordinal day. |
| [getMonthlyOrdinalNumber()](#getMonthlyOrdinalNumber--) | Gets an ordinal number of the monthly recurrence pattern. |
| [getMonthlyOrdinalRepetitions()](#getMonthlyOrdinalRepetitions--) | Gets a number of repetitions for the monthly recurrence pattern when using ordinal day. |
| [getMonthlyRepetitions()](#getMonthlyRepetitions--) | Gets a number of repetitions for the monthly recurrence pattern. |
| [getMonthlyUseOrdinalDay()](#getMonthlyUseOrdinalDay--) | Gets a value indicating whether to use ordinal day for the monthly recurrence pattern. |
| [getOccurrences()](#getOccurrences--) | Gets a number of occurrences of the recurring task. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Gets a recurrence pattern of the recurring task. |
| [getStartDate()](#getStartDate--) | Gets the date for the occurrences to begin. |
| [getTask()](#getTask--) | Gets the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class. |
| [getUseEndDate()](#getUseEndDate--) | Gets a value indicating whether to use the end date or a number of occurrences for the recurring task. |
| [getWeeklyDays()](#getWeeklyDays--) | Gets a collection of days used in the weekly recurrence pattern. |
| [getWeeklyRepetitions()](#getWeeklyRepetitions--) | Gets a number of repetitions for the weekly recurrence pattern. |
| [getYearlyDate()](#getYearlyDate--) | Gets a date for the yearly recurrence pattern. |
| [getYearlyOrdinalDay()](#getYearlyOrdinalDay--) | Gets a weekday of the yearly recurrence pattern when using ordinal day. |
| [getYearlyOrdinalMonth()](#getYearlyOrdinalMonth--) | Gets a month of the yearly recurrence pattern when using ordinal day. |
| [getYearlyOrdinalNumber()](#getYearlyOrdinalNumber--) | Gets an ordinal number of the yearly recurrence pattern. |
| [getYearlyUseOrdinalDay()](#getYearlyUseOrdinalDay--) | Gets a value indicating whether to use ordinal day for the yearly recurrence pattern. |
| [setDailyRepetitions(int value)](#setDailyRepetitions-int-) | Sets a number of repetitions for the daily recurrence pattern. |
| [setDailyUseWorkdays(boolean value)](#setDailyUseWorkdays-boolean-) | Sets a value indicating whether to use workdays for the daily recurrence pattern. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Sets the duration for one occurrence of the recurring task. |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Sets the date for the occurrences to end. |
| [setMonthlyDay(int value)](#setMonthlyDay-int-) | Sets a number of day of the monthly recurrence pattern. |
| [setMonthlyOrdinalDay(int value)](#setMonthlyOrdinalDay-int-) | Sets a day of the monthly recurrence pattern when using ordinal day. |
| [setMonthlyOrdinalNumber(int value)](#setMonthlyOrdinalNumber-int-) | Sets an ordinal number of the monthly recurrence pattern. |
| [setMonthlyOrdinalRepetitions(int value)](#setMonthlyOrdinalRepetitions-int-) | Sets a number of repetitions for the monthly recurrence pattern when using ordinal day. |
| [setMonthlyRepetitions(int value)](#setMonthlyRepetitions-int-) | Sets a number of repetitions for the monthly recurrence pattern. |
| [setMonthlyUseOrdinalDay(boolean value)](#setMonthlyUseOrdinalDay-boolean-) | Sets a value indicating whether to use ordinal day for the monthly recurrence pattern. |
| [setOccurrences(int value)](#setOccurrences-int-) | Sets a number of occurrences of the recurring task. |
| [setRecurrencePattern(int value)](#setRecurrencePattern-int-) | Sets a recurrence pattern of the recurring task. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Sets the date for the occurrences to begin. |
| [setUseEndDate(boolean value)](#setUseEndDate-boolean-) | Sets a value indicating whether to use the end date or a number of occurrences for the recurring task. |
| [setWeeklyDays(int value)](#setWeeklyDays-int-) | Sets a collection of days used in the weekly recurrence pattern. |
| [setWeeklyRepetitions(int value)](#setWeeklyRepetitions-int-) | Sets a number of repetitions for the weekly recurrence pattern. |
| [setYearlyDate(Date value)](#setYearlyDate-java.util.Date-) | Sets a date for the yearly recurrence pattern. |
| [setYearlyOrdinalDay(int value)](#setYearlyOrdinalDay-int-) | Sets a weekday of the yearly recurrence pattern when using ordinal day. |
| [setYearlyOrdinalMonth(int value)](#setYearlyOrdinalMonth-int-) | Sets a month of the yearly recurrence pattern when using ordinal day. |
| [setYearlyOrdinalNumber(int value)](#setYearlyOrdinalNumber-int-) | Sets an ordinal number of the yearly recurrence pattern. |
| [setYearlyUseOrdinalDay(boolean value)](#setYearlyUseOrdinalDay-boolean-) | Sets a value indicating whether to use ordinal day for the yearly recurrence pattern. |
### getDailyRepetitions() {#getDailyRepetitions--}
```
public final int getDailyRepetitions()
```


Gets a number of repetitions for the daily recurrence pattern.

**Returns:**
int - a number of repetitions for the daily recurrence pattern.
### getDailyUseWorkdays() {#getDailyUseWorkdays--}
```
public final boolean getDailyUseWorkdays()
```


Gets a value indicating whether to use workdays for the daily recurrence pattern.

**Returns:**
boolean - a value indicating whether to use workdays for the daily recurrence pattern.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Gets the duration for one occurrence of the recurring task.

--------------------

the instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)) class.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration for one occurrence of the recurring task.
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Gets the date for the occurrences to end.

**Returns:**
java.util.Date - the date for the occurrences to end.
### getMonthlyDay() {#getMonthlyDay--}
```
public final int getMonthlyDay()
```


Gets a number of day of the monthly recurrence pattern.

**Returns:**
int - a number of day of the monthly recurrence pattern.
### getMonthlyOrdinalDay() {#getMonthlyOrdinalDay--}
```
public final int getMonthlyOrdinalDay()
```


Gets a day of the monthly recurrence pattern when using ordinal day.

--------------------

Can be one of the values of [DayOfWeek](../../com.aspose.tasks/dayofweek) enumeration.

**Returns:**
int - a day of the monthly recurrence pattern when using ordinal day.
### getMonthlyOrdinalNumber() {#getMonthlyOrdinalNumber--}
```
public final int getMonthlyOrdinalNumber()
```


Gets an ordinal number of the monthly recurrence pattern.

--------------------

Can be one of the values of [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeration.

**Returns:**
int - an ordinal number of the monthly recurrence pattern.
### getMonthlyOrdinalRepetitions() {#getMonthlyOrdinalRepetitions--}
```
public final int getMonthlyOrdinalRepetitions()
```


Gets a number of repetitions for the monthly recurrence pattern when using ordinal day.

**Returns:**
int - a number of repetitions for the monthly recurrence pattern when using ordinal day.
### getMonthlyRepetitions() {#getMonthlyRepetitions--}
```
public final int getMonthlyRepetitions()
```


Gets a number of repetitions for the monthly recurrence pattern.

**Returns:**
int - a number of repetitions for the monthly recurrence pattern.
### getMonthlyUseOrdinalDay() {#getMonthlyUseOrdinalDay--}
```
public final boolean getMonthlyUseOrdinalDay()
```


Gets a value indicating whether to use ordinal day for the monthly recurrence pattern.

**Returns:**
boolean - a value indicating whether to use ordinal day for the monthly recurrence pattern.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Gets a number of occurrences of the recurring task.

**Returns:**
int - a number of occurrences of the recurring task.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final int getRecurrencePattern()
```


Gets a recurrence pattern of the recurring task.

--------------------

Can be one of the values of `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)) enumeration.

**Returns:**
int - a recurrence pattern of the recurring task.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Gets the date for the occurrences to begin.

**Returns:**
java.util.Date - the date for the occurrences to begin.
### getTask() {#getTask--}
```
public final Task getTask()
```


Gets the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.
### getUseEndDate() {#getUseEndDate--}
```
public final boolean getUseEndDate()
```


Gets a value indicating whether to use the end date or a number of occurrences for the recurring task.

**Returns:**
boolean - a value indicating whether to use the end date or a number of occurrences for the recurring task.
### getWeeklyDays() {#getWeeklyDays--}
```
public final int getWeeklyDays()
```


Gets a collection of days used in the weekly recurrence pattern.

--------------------

**Returns:**
int - a collection of days used in the weekly recurrence pattern.
### getWeeklyRepetitions() {#getWeeklyRepetitions--}
```
public final int getWeeklyRepetitions()
```


Gets a number of repetitions for the weekly recurrence pattern.

**Returns:**
int - a number of repetitions for the weekly recurrence pattern.
### getYearlyDate() {#getYearlyDate--}
```
public final Date getYearlyDate()
```


Gets a date for the yearly recurrence pattern.

**Returns:**
java.util.Date - a date for the yearly recurrence pattern.
### getYearlyOrdinalDay() {#getYearlyOrdinalDay--}
```
public final int getYearlyOrdinalDay()
```


Gets a weekday of the yearly recurrence pattern when using ordinal day.

--------------------

Can be one of the values of [DayOfWeek](../../com.aspose.tasks/dayofweek) enumeration.

**Returns:**
int - a weekday of the yearly recurrence pattern when using ordinal day.
### getYearlyOrdinalMonth() {#getYearlyOrdinalMonth--}
```
public final int getYearlyOrdinalMonth()
```


Gets a month of the yearly recurrence pattern when using ordinal day.

--------------------

Can be one of the values of [Month](../../com.aspose.tasks/month) enumeration.

**Returns:**
int - a month of the yearly recurrence pattern when using ordinal day.
### getYearlyOrdinalNumber() {#getYearlyOrdinalNumber--}
```
public final int getYearlyOrdinalNumber()
```


Gets an ordinal number of the yearly recurrence pattern.

--------------------

Can be one of the values of [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeration.

**Returns:**
int - an ordinal number of the yearly recurrence pattern.
### getYearlyUseOrdinalDay() {#getYearlyUseOrdinalDay--}
```
public final boolean getYearlyUseOrdinalDay()
```


Gets a value indicating whether to use ordinal day for the yearly recurrence pattern.

**Returns:**
boolean - a value indicating whether to use ordinal day for the yearly recurrence pattern.
### setDailyRepetitions(int value) {#setDailyRepetitions-int-}
```
public final void setDailyRepetitions(int value)
```


Sets a number of repetitions for the daily recurrence pattern.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a number of repetitions for the daily recurrence pattern. |

### setDailyUseWorkdays(boolean value) {#setDailyUseWorkdays-boolean-}
```
public final void setDailyUseWorkdays(boolean value)
```


Sets a value indicating whether to use workdays for the daily recurrence pattern.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to use workdays for the daily recurrence pattern. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Sets the duration for one occurrence of the recurring task.

--------------------

the instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | the duration for one occurrence of the recurring task. |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Sets the date for the occurrences to end.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | the date for the occurrences to end. |

### setMonthlyDay(int value) {#setMonthlyDay-int-}
```
public final void setMonthlyDay(int value)
```


Sets a number of day of the monthly recurrence pattern.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a number of day of the monthly recurrence pattern. |

### setMonthlyOrdinalDay(int value) {#setMonthlyOrdinalDay-int-}
```
public final void setMonthlyOrdinalDay(int value)
```


Sets a day of the monthly recurrence pattern when using ordinal day.

--------------------

Can be one of the values of [DayOfWeek](../../com.aspose.tasks/dayofweek) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a day of the monthly recurrence pattern when using ordinal day. |

### setMonthlyOrdinalNumber(int value) {#setMonthlyOrdinalNumber-int-}
```
public final void setMonthlyOrdinalNumber(int value)
```


Sets an ordinal number of the monthly recurrence pattern.

--------------------

Can be one of the values of [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | an ordinal number of the monthly recurrence pattern. |

### setMonthlyOrdinalRepetitions(int value) {#setMonthlyOrdinalRepetitions-int-}
```
public final void setMonthlyOrdinalRepetitions(int value)
```


Sets a number of repetitions for the monthly recurrence pattern when using ordinal day.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a number of repetitions for the monthly recurrence pattern when using ordinal day. |

### setMonthlyRepetitions(int value) {#setMonthlyRepetitions-int-}
```
public final void setMonthlyRepetitions(int value)
```


Sets a number of repetitions for the monthly recurrence pattern.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a number of repetitions for the monthly recurrence pattern. |

### setMonthlyUseOrdinalDay(boolean value) {#setMonthlyUseOrdinalDay-boolean-}
```
public final void setMonthlyUseOrdinalDay(boolean value)
```


Sets a value indicating whether to use ordinal day for the monthly recurrence pattern.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to use ordinal day for the monthly recurrence pattern. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Sets a number of occurrences of the recurring task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a number of occurrences of the recurring task. |

### setRecurrencePattern(int value) {#setRecurrencePattern-int-}
```
public final void setRecurrencePattern(int value)
```


Sets a recurrence pattern of the recurring task.

--------------------

Can be one of the values of `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a recurrence pattern of the recurring task. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Sets the date for the occurrences to begin.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | the date for the occurrences to begin. |

### setUseEndDate(boolean value) {#setUseEndDate-boolean-}
```
public final void setUseEndDate(boolean value)
```


Sets a value indicating whether to use the end date or a number of occurrences for the recurring task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to use the end date or a number of occurrences for the recurring task. |

### setWeeklyDays(int value) {#setWeeklyDays-int-}
```
public final void setWeeklyDays(int value)
```


Sets a collection of days used in the weekly recurrence pattern.

--------------------

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a collection of days used in the weekly recurrence pattern. |

### setWeeklyRepetitions(int value) {#setWeeklyRepetitions-int-}
```
public final void setWeeklyRepetitions(int value)
```


Sets a number of repetitions for the weekly recurrence pattern.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a number of repetitions for the weekly recurrence pattern. |

### setYearlyDate(Date value) {#setYearlyDate-java.util.Date-}
```
public final void setYearlyDate(Date value)
```


Sets a date for the yearly recurrence pattern.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a date for the yearly recurrence pattern. |

### setYearlyOrdinalDay(int value) {#setYearlyOrdinalDay-int-}
```
public final void setYearlyOrdinalDay(int value)
```


Sets a weekday of the yearly recurrence pattern when using ordinal day.

--------------------

Can be one of the values of [DayOfWeek](../../com.aspose.tasks/dayofweek) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a weekday of the yearly recurrence pattern when using ordinal day. |

### setYearlyOrdinalMonth(int value) {#setYearlyOrdinalMonth-int-}
```
public final void setYearlyOrdinalMonth(int value)
```


Sets a month of the yearly recurrence pattern when using ordinal day.

--------------------

Can be one of the values of [Month](../../com.aspose.tasks/month) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a month of the yearly recurrence pattern when using ordinal day. |

### setYearlyOrdinalNumber(int value) {#setYearlyOrdinalNumber-int-}
```
public final void setYearlyOrdinalNumber(int value)
```


Sets an ordinal number of the yearly recurrence pattern.

--------------------

Can be one of the values of [OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | an ordinal number of the yearly recurrence pattern. |

### setYearlyUseOrdinalDay(boolean value) {#setYearlyUseOrdinalDay-boolean-}
```
public final void setYearlyUseOrdinalDay(boolean value)
```


Sets a value indicating whether to use ordinal day for the yearly recurrence pattern.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to use ordinal day for the yearly recurrence pattern. |

