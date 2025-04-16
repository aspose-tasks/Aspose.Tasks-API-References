---
title: Interface ICalendar
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ICalendar interface. Represents a calendar abstraction which can be used for various calculations of dates and durations
type: docs
weight: 830
url: /net/aspose.tasks/icalendar/
---
## ICalendar interface

Represents a calendar abstraction which can be used for various calculations of dates and durations.

```csharp
public interface ICalendar
```

## Methods

| Name | Description |
| --- | --- |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Calculates the date when the specified amount of work time will pass according to the calendar. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Calculates the date when the specified amount of work time will pass according to the calendar. |
| [GetNextWorkingDayStart](../../aspose.tasks/icalendar/getnextworkingdaystart/)(DateTime) | Calculates next working day start for the specified date. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/icalendar/getpreviousworkingdayend/)(DateTime) | Calculates the end of the previous working date from the specified date. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Returns start date based on the specified finish date and duration. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Returns start date based on specified finish date and duration. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/icalendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Calculates the task finish date and time from its start date, split parts and the work duration. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours_1)(DateTime) | Returns the amount of working hours at the specified date. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Return WorkUnit - Start, Finish and Duration of working hours for the specified date time interval. |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | Returns [`WorkingTimeCollection`](../workingtimecollection/) of working times for the specified date. |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | Determines whether the specified day is a working day according to the calendar. |

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


