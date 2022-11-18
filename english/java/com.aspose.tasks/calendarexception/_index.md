---
title: CalendarException
second_title: Aspose.Tasks for Java API Reference
description: Represent exceptional time periods in a calendar.
type: docs
weight: 43
url: /java/com.aspose.tasks/calendarexception/
---

**Inheritance:**
java.lang.Object
```
public final class CalendarException
```

Represent exceptional time periods in a calendar.
## Constructors

| Constructor | Description |
| --- | --- |
| [CalendarException()](#CalendarException--) | Initializes a new instance of the [CalendarException](../../com.aspose.tasks/calendarexception) class. |
## Methods

| Method | Description |
| --- | --- |
| [checkException(Date dt)](#checkException-java.util.Date-) | Returns true if the specified instance of the java.util.Date struct is the exception day. |
| [delete()](#delete--) | Deletes the Exception instance from parent calendar CalendarExceptionCollection object. |
| [getDayWorking()](#getDayWorking--) | Gets a value indicating whether the specified date or day type is working. |
| [getDaysOfWeek()](#getDaysOfWeek--) | Gets the DayTypeCollection for this object. |
| [getEnteredByOccurrences()](#getEnteredByOccurrences--) | Gets a value indicating whether the range of recurrence is defined by entering a number of occurrences. |
| [getExceptionDates()](#getExceptionDates--) | Returns dates on which the calendar exception is applicable. |
| [getFromDate()](#getFromDate--) | Gets the beginning of the exception time. |
| [getMonth()](#getMonth--) | Gets the month for which an exception recurrence is scheduled. |
| [getMonthDay()](#getMonthDay--) | Gets the day of a month on which an exception recurrence is scheduled. |
| [getMonthItem()](#getMonthItem--) | Gets the month item for which an exception recurrence is scheduled. |
| [getMonthPosition()](#getMonthPosition--) | Gets the position of a month item within a month. |
| [getName()](#getName--) | Gets the name of the exception. |
| [getOccurrences()](#getOccurrences--) | Gets the number of occurrences for which the calendar exception is valid. |
| [getParentCalendar()](#getParentCalendar--) | Gets the parent calendar for this object. |
| [getPeriod()](#getPeriod--) | Gets the period of recurrence for the exception. |
| [getToDate()](#getToDate--) | Gets the end of the exception time. |
| [getType()](#getType--) | Gets the exception type. |
| [getWorkingTime()](#getWorkingTime--) | Returns the working time for a calendar exception. |
| [getWorkingTimes()](#getWorkingTimes--) | Gets the WorkingTimeCollection object. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Sets a value indicating whether the specified date or day type is working. |
| [setEnteredByOccurrences(boolean value)](#setEnteredByOccurrences-boolean-) | Sets a value indicating whether the range of recurrence is defined by entering a number of occurrences. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Sets the beginning of the exception time. |
| [setMonth(int value)](#setMonth-int-) | Sets the month for which an exception recurrence is scheduled. |
| [setMonthDay(int value)](#setMonthDay-int-) | Sets the day of a month on which an exception recurrence is scheduled. |
| [setMonthItem(int value)](#setMonthItem-int-) | Sets the month item for which an exception recurrence is scheduled. |
| [setMonthPosition(int value)](#setMonthPosition-int-) | Sets the position of a month item within a month. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the exception. |
| [setOccurrences(int value)](#setOccurrences-int-) | Sets the number of occurrences for which the calendar exception is valid. |
| [setPeriod(int value)](#setPeriod-int-) | Sets the period of recurrence for the exception. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Sets the end of the exception time. |
| [setType(int value)](#setType-int-) | Sets the exception type. |
| [setWorkingTimes(WorkingTimeCollection value)](#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-) | Sets the WorkingTimeCollection object. |
### CalendarException() {#CalendarException--}
```
public CalendarException()
```


Initializes a new instance of the [CalendarException](../../com.aspose.tasks/calendarexception) class.

### checkException(Date dt) {#checkException-java.util.Date-}
```
public final boolean checkException(Date dt)
```


Returns true if the specified instance of the java.util.Date struct is the exception day.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dt | java.util.Date | the specified instance of the java.util.Date struct. |

**Returns:**
boolean - Returns true if java.util.Date value is the exception day; otherwise, false.
### delete() {#delete--}
```
public final void delete()
```


Deletes the Exception instance from parent calendar CalendarExceptionCollection object.

### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Gets a value indicating whether the specified date or day type is working.

**Returns:**
boolean - a value indicating whether the specified date or day type is working.
### getDaysOfWeek() {#getDaysOfWeek--}
```
public final DayTypeCollection getDaysOfWeek()
```


Gets the DayTypeCollection for this object. The days of the week on which the exception is valid.

**Returns:**
[DayTypeCollection](../../com.aspose.tasks/daytypecollection) - the DayTypeCollection for this object.
### getEnteredByOccurrences() {#getEnteredByOccurrences--}
```
public final boolean getEnteredByOccurrences()
```


Gets a value indicating whether the range of recurrence is defined by entering a number of occurrences. False specifies that the range of recurrence is defined by entering a finish date.

**Returns:**
boolean - a value indicating whether the range of recurrence is defined by entering a number of occurrences.
### getExceptionDates() {#getExceptionDates--}
```
public final Iterable<Date> getExceptionDates()
```


Returns dates on which the calendar exception is applicable.

**Returns:**
java.lang.Iterable&lt;java.util.Date&gt; - dates on which the calendar exception is applicable.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Gets the beginning of the exception time.

**Returns:**
java.util.Date - the beginning of the exception time.
### getMonth() {#getMonth--}
```
public final int getMonth()
```


Gets the month for which an exception recurrence is scheduled.

**Returns:**
int - the month for which an exception recurrence is scheduled.
### getMonthDay() {#getMonthDay--}
```
public final int getMonthDay()
```


Gets the day of a month on which an exception recurrence is scheduled.

**Returns:**
int - the day of a month on which an exception recurrence is scheduled.
### getMonthItem() {#getMonthItem--}
```
public final int getMonthItem()
```


Gets the month item for which an exception recurrence is scheduled.

**Returns:**
int - the month item for which an exception recurrence is scheduled.
### getMonthPosition() {#getMonthPosition--}
```
public final int getMonthPosition()
```


Gets the position of a month item within a month.

**Returns:**
int - the position of a month item within a month.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the exception.

**Returns:**
java.lang.String - the name of the exception.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Gets the number of occurrences for which the calendar exception is valid.

**Returns:**
int - the number of occurrences for which the calendar exception is valid.
### getParentCalendar() {#getParentCalendar--}
```
public final Calendar getParentCalendar()
```


Gets the parent calendar for this object.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the parent calendar for this object.
### getPeriod() {#getPeriod--}
```
public final int getPeriod()
```


Gets the period of recurrence for the exception.

**Returns:**
int - the period of recurrence for the exception.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Gets the end of the exception time.

**Returns:**
java.util.Date - the end of the exception time.
### getType() {#getType--}
```
public final int getType()
```


Gets the exception type.

**Returns:**
int - the exception type.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Returns the working time for a calendar exception.

**Returns:**
double - Returns working time for this calendar exception.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Gets the WorkingTimeCollection object. The collection of working times that defines the time worked on the weekday.

--------------------

At least one working time must present, and there can't be more than five.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - the WorkingTimeCollection object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Sets a value indicating whether the specified date or day type is working.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the specified date or day type is working. |

### setEnteredByOccurrences(boolean value) {#setEnteredByOccurrences-boolean-}
```
public final void setEnteredByOccurrences(boolean value)
```


Sets a value indicating whether the range of recurrence is defined by entering a number of occurrences. False specifies that the range of recurrence is defined by entering a finish date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the range of recurrence is defined by entering a number of occurrences. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Sets the beginning of the exception time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | the beginning of the exception time. |

### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


Sets the month for which an exception recurrence is scheduled.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the month for which an exception recurrence is scheduled. |

### setMonthDay(int value) {#setMonthDay-int-}
```
public final void setMonthDay(int value)
```


Sets the day of a month on which an exception recurrence is scheduled.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the day of a month on which an exception recurrence is scheduled. |

### setMonthItem(int value) {#setMonthItem-int-}
```
public final void setMonthItem(int value)
```


Sets the month item for which an exception recurrence is scheduled.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the month item for which an exception recurrence is scheduled. |

### setMonthPosition(int value) {#setMonthPosition-int-}
```
public final void setMonthPosition(int value)
```


Sets the position of a month item within a month.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the position of a month item within a month. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the exception.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the exception. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Sets the number of occurrences for which the calendar exception is valid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of occurrences for which the calendar exception is valid. |

### setPeriod(int value) {#setPeriod-int-}
```
public final void setPeriod(int value)
```


Sets the period of recurrence for the exception.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the period of recurrence for the exception. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Sets the end of the exception time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | the end of the exception time. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Sets the exception type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the exception type. |

### setWorkingTimes(WorkingTimeCollection value) {#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-}
```
public final void setWorkingTimes(WorkingTimeCollection value)
```


Sets the WorkingTimeCollection object. The collection of working times that defines the time worked on the weekday.

--------------------

At least one working time must present, and there can't be more than five.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) | the WorkingTimeCollection object. |

