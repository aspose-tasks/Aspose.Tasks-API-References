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
```
public class Calendar
```

Represents a calendar used in a project.

--------------------

&gt; ```
&gt; How to create simple calendar from scratch.
&gt;  ```
&gt; 
&gt;  // create empty calendar
&gt;  Calendar calendar = new Calendar();
&gt;  // adds default working days (8 working hours from 9:00 to 17:00)
&gt;  calendar.getDays().add(WeekDay.createDefaultWorkingDay(DayType.Monday));
&gt;  calendar.getDays().add(WeekDay.createDefaultWorkingDay(DayType.Tuesday));
&gt;  calendar.getDays().add(WeekDay.createDefaultWorkingDay(DayType.Wednesday));
&gt;  // create new new working day
&gt;  WeekDay myWeekDay = new WeekDay(DayType.Thursday);
&gt;  // Sets working time. Only time part of DateTime is important
&gt;  WorkingTime wt1 = new WorkingTime();
&gt;  wt1.setFromTime(new Date(1, 1, 1, 6, 0, 0));
&gt;  wt1.setToTime(new Date(1, 1, 1, 12, 0, 0));
&gt;  WorkingTime wt2 = new WorkingTime();
&gt;  wt2.setFromTime(new Date(1, 1, 1, 14, 0, 0));
&gt;  wt2.setToTime(new Date(1, 1, 1, 18, 0, 0));
&gt;  myWeekDay.getWorkingTimes().add(wt1);
&gt;  myWeekDay.getWorkingTimes().add(wt2);
&gt;  myWeekDay.setDayWorking(true);
&gt;  calendar.getDays().add(myWeekDay);
&gt;  calendar.getDays().add(WeekDay.createDefaultWorkingDay(DayType.Friday));
&gt;  // adds weekend
&gt;  calendar.getDays().add(new WeekDay(DayType.Saturday));
&gt;  calendar.getDays().add(new WeekDay(DayType.Sunday));
&gt;  
&gt; ```
&gt; ```

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
| [getName()](#getName--) | Gets the name of the calendar. |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | Calculates next working day start from the date. |
| [getParentProject()](#getParentProject--) | Gets parent project for this calendar. |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | Calculates previous working date end from the specified date. |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | Returns StartDate based on specified FinishDate and Duration. |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | Returns StartDate based on specified FinishDate and Duration. |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | Calculates the task finish date and time from its start date, split parts and the duration. |
| [getUid()](#getUid--) | Gets the unique identifier of the calendar. |
| [getWeekDays()](#getWeekDays--) | Gets WeekDaysCollection for this calendar. |
| [getWorkWeeks()](#getWorkWeeks--) | Gets WorkWeekCollections object. |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | Returns amount of working hours at the date. |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | Return working hours for the specified dates. |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | Returns [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) of working times for the specified date. |
| [hashCode()](#hashCode--) | Returns a hash code for the instance of the class. |
| [isBaseCalendar()](#isBaseCalendar--) | Gets a value indicating whether the calendar is a base calendar. |
| [isBaselineCalendar()](#isBaselineCalendar--) | Gets a value indicating whether the calendar is a baseline calendar. |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | Determines whether the day is working day. |
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


Calculates next working day start from the date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| date | java.util.Date | The date to get next working day start for. |

**Returns:**
java.util.Date - Next working day start java.util.Date.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets parent project for this calendar.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this calendar.
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public final Date getPreviousWorkingDayEnd(Date date)
```


Calculates previous working date end from the specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| date | java.util.Date | the specified instance of java.util.Date struct. |

**Returns:**
java.util.Date - Previous working day start java.util.Date
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public final Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


Returns StartDate based on specified FinishDate and Duration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| finish | java.util.Date | The specified finish date. |
| duration | [Duration](../../com.aspose.tasks/duration) | The specified work duration. |

**Returns:**
java.util.Date - Calculated StartDate.
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public final Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


Returns StartDate based on specified FinishDate and Duration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| finish | java.util.Date | The specified finish date. |
| duration | double | The specified work duration. |

**Returns:**
java.util.Date - Calculated StartDate.
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public final Date getTaskFinishDateFromDuration(Task task, double duration)
```


Calculates the task finish date and time from its start date, split parts and the duration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | The task to get finish date for. |
| duration | double | The task duration to split on.

--------------------

Returns DateTime.MinValue if task is summary, null or its start date is not set. |

**Returns:**
java.util.Date - Task's finish date.
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


Returns amount of working hours at the date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dt | java.util.Date | The date to get working hours for. |

**Returns:**
double - Working hours.
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public final WorkUnit getWorkingHours(Date start, Date finish)
```


Return working hours for the specified dates.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | Start date. |
| finish | java.util.Date | Finish date. |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Working hours.
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
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - List of [WorkingTime](../../com.aspose.tasks/workingtime).
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


Determines whether the day is working day.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dt | java.util.Date | The date to check day is working for. |

**Returns:**
boolean - True if the day is working day.
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

