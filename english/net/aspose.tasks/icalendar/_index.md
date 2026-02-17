---
title: Interface ICalendar
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ICalendar interface. Represents a calendar abstraction which can be used for various calculations of dates and durations
type: docs
weight: 840
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
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Returns WorkUnit - Start, Finish and Duration of working hours for the specified date time interval. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/icalendar/getworkinghourstimespan/)(DateTime, DateTime) | Returns amount of working hours between the specified dates. |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | Returns [`WorkingTimeCollection`](../workingtimecollection/) of working times for the specified date. |
| [GetWorkStart](../../aspose.tasks/icalendar/getworkstart/)(DateTime) | Calculates next working time start beginning from the specified date and time. |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | Determines whether the specified day is a working day according to the calendar. |
| [IsEmpty](../../aspose.tasks/icalendar/isempty/)() | Returns whether the calendar doesn't have working hours defined. |

## Examples

Shows how to use Calendar.GetIntersectionCalendar() method to perform calculation on assignment's calendar.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

foreach (var ra in project.ResourceAssignments)
{
    if (ra.Resource == null)
    {
        continue;
    }

    ICalendar assignmentCalendar;

    Calendar taskCalendar = ra.Task.Calendar != null && !ra.Task.Duration.IsEstimated ? ra.Task.Calendar : null;
    Calendar resourceCalendar = ra.Resource.Calendar != null && !ra.Task.IgnoreResourceCalendar
        ? ra.Resource.Calendar
        : null;

    if (taskCalendar != null && resourceCalendar != null && !ReferenceEquals(taskCalendar, resourceCalendar))
    {
        assignmentCalendar = Calendar.GetIntersectionCalendar(taskCalendar, resourceCalendar);
    }
    else
    {
        assignmentCalendar = taskCalendar ?? resourceCalendar;
    }

    if (assignmentCalendar == null)
    {
        assignmentCalendar = project.Calendar;
    }

    var workingHours = assignmentCalendar.GetWorkingHours(ra.Start, ra.Finish);

    Console.WriteLine("Working hours for assignment '{0}' : {1}", ra, workingHours);

    var date = new DateTime(2025, 4, 7);
    Console.WriteLine("Working times for date '{0}':", date);

    foreach (var wt in assignmentCalendar.GetWorkingTimes(date))
    {
        Console.WriteLine("{0} - {1}", wt.From.TimeOfDay, wt.To.TimeOfDay);
    }
}
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


