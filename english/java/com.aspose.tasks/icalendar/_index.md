---
title: ICalendar
second_title: Aspose.Tasks for Java API Reference
description: Represents a calendar abstraction which can be used for various calculations of dates and durations.
type: docs
weight: 375
url: /java/com.aspose.tasks/icalendar/
---
```
public interface ICalendar
```

Represents a calendar abstraction which can be used for various calculations of dates and durations.
## Methods

| Method | Description |
| --- | --- |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | Calculates the date when the specified amount of work time will pass according to the calendar. |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | Calculates the date when the specified amount of work time will pass according to the calendar. |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | Calculates next working day start for the specified date. |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | Calculates the end of the previous working date from the specified date. |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | Returns start date based on the specified finish date and duration. |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | Returns start date based on specified finish date and duration. |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | Calculates the task finish date and time from its start date, split parts and the work duration. |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | Calculates next working time start beginning from the specified date and time. |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | Returns the amount of working hours at the specified date. |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | Return WorkUnit - Start, Finish and Duration of working hours for the specified date time interval. |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | Returns amount of working hours between the specified dates. |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | Returns [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) of working times for the specified date. |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | Determines whether the specified day is a working day according to the calendar. |
| [isEmpty()](#isEmpty--) | Returns whether the calendar doesn't have working hours defined. |
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getFinishDateByStartAndWork(Date start, Duration work)
```


Calculates the date when the specified amount of work time will pass according to the calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | Start date. |
| work | [Duration](../../com.aspose.tasks/duration) | Work duration. |

**Returns:**
java.util.Date - Finish date.
### getFinishDateByStartAndWork(Date start, double work) {#getFinishDateByStartAndWork-java.util.Date-double-}
```
public abstract Date getFinishDateByStartAndWork(Date start, double work)
```


Calculates the date when the specified amount of work time will pass according to the calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | Start date. |
| work | double | Work duration. |

**Returns:**
java.util.Date - Finish date.
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public abstract Date getNextWorkingDayStart(Date date)
```


Calculates next working day start for the specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| date | java.util.Date | The date to get next working day start for. |

**Returns:**
java.util.Date - Next working day start System.DateTime.
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public abstract Date getPreviousWorkingDayEnd(Date date)
```


Calculates the end of the previous working date from the specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| date | java.util.Date | the date to calculate the previous working day end. |

**Returns:**
java.util.Date - The end of the previous working day end
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


Returns start date based on the specified finish date and duration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| finish | java.util.Date | The specified finish date. |
| duration | [Duration](../../com.aspose.tasks/duration) | The specified duration. |

**Returns:**
java.util.Date - Calculated start date.
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


Returns start date based on specified finish date and duration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| finish | java.util.Date | The specified finish date. |
| duration | double | The specified duration. |

**Returns:**
java.util.Date - Calculated start date.
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public abstract Date getTaskFinishDateFromDuration(Task task, double duration)
```


Calculates the task finish date and time from its start date, split parts and the work duration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | The task to calculate finish date for. |
| duration | double | The duration to calculate.

Returns DateTime.MinValue if task is summary, null or its start date is not set. |

**Returns:**
java.util.Date - Task's finish date for the given start date and duration.
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public abstract Date getWorkStart(Date date)
```


Calculates next working time start beginning from the specified date and time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| date | java.util.Date | The date and time. |

**Returns:**
java.util.Date - The nearest working time start.
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public abstract double getWorkingHours(Date dt)
```


Returns the amount of working hours at the specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dt | java.util.Date | The date to get working hours for. |

**Returns:**
double - Working hours at the specified date.
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public abstract WorkUnit getWorkingHours(Date start, Date finish)
```


Return WorkUnit - Start, Finish and Duration of working hours for the specified date time interval.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | Start date of the interval. |
| finish | java.util.Date | Finish date of the interval. |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Instance of [WorkUnit](../../com.aspose.tasks/workunit) class containing Start, Finish and Duration of working hours.
### getWorkingHoursTimeSpan(Date start, Date finish) {#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-}
```
public abstract double getWorkingHoursTimeSpan(Date start, Date finish)
```


Returns amount of working hours between the specified dates.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | Start date of the interval. |
| finish | java.util.Date | Finish date of the interval. |

**Returns:**
double - Amount of working hours according to the calendar instance.
### getWorkingTimes(Date dt) {#getWorkingTimes-java.util.Date-}
```
public abstract WorkingTimeCollection getWorkingTimes(Date dt)
```


Returns [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) of working times for the specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dt | java.util.Date | The date to get working times for. |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public abstract boolean isDayWorking(Date dt)
```


Determines whether the specified day is a working day according to the calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dt | java.util.Date | The date to check whether the day is working. |

**Returns:**
boolean - True if the day is a working day.
### isEmpty() {#isEmpty--}
```
public abstract boolean isEmpty()
```


Returns whether the calendar doesn't have working hours defined.

**Returns:**
boolean - True if the calendar doesn't have working hours defined.
