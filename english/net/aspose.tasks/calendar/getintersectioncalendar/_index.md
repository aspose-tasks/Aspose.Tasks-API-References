---
title: Calendar.GetIntersectionCalendar
second_title: Aspose.Tasks for .NET API Reference
description: Calendar method. Gets ICalendar instance which can be used to perform calculations on the intersection of work schedules of 2 calendars
type: docs
weight: 280
url: /net/aspose.tasks/calendar/getintersectioncalendar/
---
## Calendar.GetIntersectionCalendar method

Gets [`ICalendar`](../../icalendar/) instance which can be used to perform calculations on the intersection of work schedules of 2 calendars.

```csharp
public static ICalendar GetIntersectionCalendar(Calendar calendar1, Calendar calendar2)
```

| Parameter | Type | Description |
| --- | --- | --- |
| calendar1 | Calendar | First calendar. |
| calendar2 | Calendar | Second calendar. |

### Return Value

Implementation of ICalendar interface.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | When any of the arguments is null. |

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

* interface [ICalendar](../../icalendar/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


