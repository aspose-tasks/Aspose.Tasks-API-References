---
title: Calendar
second_title: Aspose.Tasks for Java API Reference
description: Represents a calendar used in a project.
type: docs
weight: 41
url: /java/com.aspose.tasks/calendar/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.tasks.ICalendar](../../com.aspose.tasks/icalendar)
```
public class Calendar implements ICalendar
```

Represents a calendar used in a project.

--------------------

&gt; ```
&gt; How to create simple calendar from scratch.
&gt; ``````

 // create empty calendar
 Calendar calendar = new Calendar();
 // adds default working days (8 working hours from 9:00 to 17:00)
 calendar.getDays().add(WeekDay.createDefaultWorkingDay(DayType.Monday));
 calendar.getDays().add(WeekDay.createDefaultWorkingDay(DayType.Tuesday));
 calendar.getDays().add(WeekDay.createDefaultWorkingDay(DayType.Wednesday));
 // create new new working day
 WeekDay myWeekDay = new WeekDay(DayType.Thursday);
 // Sets working time. Only time part of DateTime is important
 WorkingTime wt1 = new WorkingTime();
 wt1.setFromTime(new Date(1, 1, 1, 6, 0, 0));
 wt1.setToTime(new Date(1, 1, 1, 12, 0, 0));
 WorkingTime wt2 = new WorkingTime();
 wt2.setFromTime(new Date(1, 1, 1, 14, 0, 0));
 wt2.setToTime(new Date(1, 1, 1, 18, 0, 0));
 myWeekDay.getWorkingTimes().add(wt1);
 myWeekDay.getWorkingTimes().add(wt2);
 myWeekDay.setDayWorking(true);
 calendar.getDays().add(myWeekDay);
 calendar.getDays().add(WeekDay.createDefaultWorkingDay(DayType.Friday));
 // adds weekend
 calendar.getDays().add(new WeekDay(DayType.Saturday));
 calendar.getDays().add(new WeekDay(DayType.Sunday));
 
```

--------------------

Calendars are used to define standard working and non-working times. Projects must have one base calendar. Tasks and resources can have their own non-base calendars that are based on a base calendar.
## Methods

| Method | Description |
| --- | --- |
| [delete()](#delete--) | Removes calendar from project. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [getBaseCalendar()](#getBaseCalendar--) | Gets the base calendar on which this calendar depends. |
| [getExceptions()](#getExceptions--) | Gets CalendarExceptionCollection object. |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | Calculates the date when the specified amount of work time will pass according to the calendar. |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | Calculates the date when the specified amount of work time will pass according to the calendar. |
| [getGuid()](#getGuid--) | Gets calendar's Guid. |
| [getIntersectionCalendar(Calendar calendar1, Calendar calendar2)](#getIntersectionCalendar-com.aspose.tasks.Calendar-com.aspose.tasks.Calendar-) | Gets [ICalendar](../../com.aspose.tasks/icalendar) instance which can be used to perform calculations on the intersection of work schedules of 2 calendars. |
| [getName()](#getName--) | Gets the name of the calendar. |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | Calculates next working day start for the specified date. |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | Calculates the end of the previous working date from the specified date. |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | Gets an object containing Primavera-specific properties for a calendar read from Primavera formats. |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | Returns start date based on the specified finish date and duration. |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | Returns start date based on specified finish date and duration. |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | Calculates the task finish date and time from its start date, split parts and the work duration. |
| [getUid()](#getUid--) | Gets the unique identifier of the calendar. |
| [getWeekDays()](#getWeekDays--) | Gets WeekDaysCollection for this calendar. |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | Calculates next working time start beginning from the specified date and time. |
| [getWorkWeeks()](#getWorkWeeks--) | Gets WorkWeekCollections object. |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | Returns the amount of working hours at the specified date. |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | Return WorkUnit - Start, Finish and Duration of working hours for the specified date time interval. |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | Returns amount of working hours between the specified dates. |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | Returns [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) of working times for the specified date. |
| [hashCode()](#hashCode--) | Returns a hash code for the instance of the class. |
| [isBaseCalendar()](#isBaseCalendar--) | Gets a value indicating whether the calendar is a base calendar. |
| [isBaselineCalendar()](#isBaselineCalendar--) | Gets a value indicating whether the calendar is a baseline calendar. |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | Determines whether the specified day is a working day according to the calendar. |
| [isEmpty()](#isEmpty--) | Returns whether the calendar doesn't have working hours defined. |
| [make24HourCalendar(Calendar calendar)](#make24HourCalendar-com.aspose.tasks.Calendar-) | Makes a given Calendar to be a 24Hour Calendar. |
| [makeNightShiftCalendar(Calendar calendar)](#makeNightShiftCalendar-com.aspose.tasks.Calendar-) | Makes a given Calendar as Night Shift Calendar. |
| [makeStandardCalendar(Calendar calendar)](#makeStandardCalendar-com.aspose.tasks.Calendar-) | Creates default standard calendar. |
| [setBaseCalendar(Calendar value)](#setBaseCalendar-com.aspose.tasks.Calendar-) | Sets the base calendar on which this calendar depends. |
| [setBaselineCalendar(boolean value)](#setBaselineCalendar-boolean-) | Sets a value indicating whether the calendar is a baseline calendar. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the calendar. |
| [setUid(int value)](#setUid-int-) | Sets the unique identifier of the calendar. |
### delete() {#delete--}
```
public final void delete()
```


Removes calendar from project.

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
boolean - **True** if o is a Calendar that has the same Uid value as this instance; otherwise, **false**.
### getBaseCalendar() {#getBaseCalendar--}
```
public final Calendar getBaseCalendar()
```


Gets the base calendar on which this calendar depends. Only applicable if the calendar is not a base calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the base calendar on which this calendar depends.
### getExceptions() {#getExceptions--}
```
public final CalendarExceptionCollection getExceptions()
```


Gets CalendarExceptionCollection object. The collection of exceptions that is associated with the calendar.

**Returns:**
[CalendarExceptionCollection](../../com.aspose.tasks/calendarexceptioncollection) - CalendarExceptionCollection object.
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public final Date getFinishDateByStartAndWork(Date start, Duration work)
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
public final Date getFinishDateByStartAndWork(Date start, double work)
```


Calculates the date when the specified amount of work time will pass according to the calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | Start date. |
| work | double | Work duration. |

**Returns:**
java.util.Date - Finish date.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Gets calendar's Guid.

**Returns:**
java.lang.String - calendar's Guid.
### getIntersectionCalendar(Calendar calendar1, Calendar calendar2) {#getIntersectionCalendar-com.aspose.tasks.Calendar-com.aspose.tasks.Calendar-}
```
public static ICalendar getIntersectionCalendar(Calendar calendar1, Calendar calendar2)
```


Gets [ICalendar](../../com.aspose.tasks/icalendar) instance which can be used to perform calculations on the intersection of work schedules of 2 calendars.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| calendar1 | [Calendar](../../com.aspose.tasks/calendar) | First calendar. |
| calendar2 | [Calendar](../../com.aspose.tasks/calendar) | Second calendar. |

**Returns:**
[ICalendar](../../com.aspose.tasks/icalendar) - Implementation of ICalendar interface.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the calendar.

**Returns:**
java.lang.String - the name of the calendar.
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public final Date getNextWorkingDayStart(Date date)
```


Calculates next working day start for the specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| date | java.util.Date | The date to get next working day start for. |

**Returns:**
java.util.Date - Next working day start java.util.Date.
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public final Date getPreviousWorkingDayEnd(Date date)
```


Calculates the end of the previous working date from the specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| date | java.util.Date | the specified instance of java.util.Date struct. |

**Returns:**
java.util.Date - The end of the previous working day end java.util.Date
### getPrimaveraProperties() {#getPrimaveraProperties--}
```
public final PrimaveraCalendarProperties getPrimaveraProperties()
```


Gets an object containing Primavera-specific properties for a calendar read from Primavera formats.

**Returns:**
[PrimaveraCalendarProperties](../../com.aspose.tasks/primaveracalendarproperties) - an object containing Primavera-specific properties for a calendar read from Primavera formats.
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public final Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
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
public final Date getStartDateFromFinishAndDuration(Date finish, double duration)
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
public final Date getTaskFinishDateFromDuration(Task task, double duration)
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
### getUid() {#getUid--}
```
public final int getUid()
```


Gets the unique identifier of the calendar.

**Returns:**
int - the unique identifier of the calendar.
### getWeekDays() {#getWeekDays--}
```
public final WeekDayCollection getWeekDays()
```


Gets WeekDaysCollection for this calendar. The collection of weekdays that defines the calendar.

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - WeekDaysCollection for this calendar.
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public final Date getWorkStart(Date date)
```


Calculates next working time start beginning from the specified date and time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| date | java.util.Date | The date and time. |

**Returns:**
java.util.Date - The nearest working time start.
### getWorkWeeks() {#getWorkWeeks--}
```
public final WorkWeekCollection getWorkWeeks()
```


Gets WorkWeekCollections object. The collection of work weeks that is associated with the calendar.

**Returns:**
[WorkWeekCollection](../../com.aspose.tasks/workweekcollection) - WorkWeekCollections object.
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public final double getWorkingHours(Date dt)
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
public final WorkUnit getWorkingHours(Date start, Date finish)
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
public final double getWorkingHoursTimeSpan(Date start, Date finish)
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
public final WorkingTimeCollection getWorkingTimes(Date dt)
```


Returns [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) of working times for the specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dt | java.util.Date | The date to get working times for. |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code for the instance of the class.

**Returns:**
int - a hash code for this object.
### isBaseCalendar() {#isBaseCalendar--}
```
public final boolean isBaseCalendar()
```


Gets a value indicating whether the calendar is a base calendar.

**Returns:**
boolean - a value indicating whether the calendar is a base calendar.
### isBaselineCalendar() {#isBaselineCalendar--}
```
public final boolean isBaselineCalendar()
```


Gets a value indicating whether the calendar is a baseline calendar.

**Returns:**
boolean - a value indicating whether the calendar is a baseline calendar.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public final boolean isDayWorking(Date dt)
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
public boolean isEmpty()
```


Returns whether the calendar doesn't have working hours defined.

**Returns:**
boolean - True if the calendar doesn't have working hours defined.
### make24HourCalendar(Calendar calendar) {#make24HourCalendar-com.aspose.tasks.Calendar-}
```
public static Calendar make24HourCalendar(Calendar calendar)
```


Makes a given Calendar to be a 24Hour Calendar. 24Hours Calendar is a Calendar in which every day of week is working with Round-the-clock working hours.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Calendar to make 24 Hours Calendar from. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - 24Hour Calendar.
### makeNightShiftCalendar(Calendar calendar) {#makeNightShiftCalendar-com.aspose.tasks.Calendar-}
```
public static Calendar makeNightShiftCalendar(Calendar calendar)
```


Makes a given Calendar as Night Shift Calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Calendar to make Night Shift Calendar. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Night Shift Calendar.
### makeStandardCalendar(Calendar calendar) {#makeStandardCalendar-com.aspose.tasks.Calendar-}
```
public static Calendar makeStandardCalendar(Calendar calendar)
```


Creates default standard calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Calendar to make standard calendar from. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Calendar with 5 working days (Monday-Friday) with working times 8-12 and 13-17.
### setBaseCalendar(Calendar value) {#setBaseCalendar-com.aspose.tasks.Calendar-}
```
public final void setBaseCalendar(Calendar value)
```


Sets the base calendar on which this calendar depends. Only applicable if the calendar is not a base calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | the base calendar on which this calendar depends. |

### setBaselineCalendar(boolean value) {#setBaselineCalendar-boolean-}
```
public final void setBaselineCalendar(boolean value)
```


Sets a value indicating whether the calendar is a baseline calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the calendar is a baseline calendar. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the calendar. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Sets the unique identifier of the calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the unique identifier of the calendar. |

