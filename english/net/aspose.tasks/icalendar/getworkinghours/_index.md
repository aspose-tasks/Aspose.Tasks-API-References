---
title: ICalendar.GetWorkingHours
second_title: Aspose.Tasks for .NET API Reference
description: ICalendar method. Returns WorkUnit  Start Finish and Duration of working hours for the specified date time interval
type: docs
weight: 60
url: /net/aspose.tasks/icalendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Returns WorkUnit - Start, Finish and Duration of working hours for the specified date time interval.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | Start date of the interval. |
| finish | DateTime | Finish date of the interval. |

### Return Value

Instance of [`WorkUnit`](../../workunit/) class containing Start, Finish and Duration of working hours.

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

* class [WorkUnit](../../workunit/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Returns the amount of working hours at the specified date.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dt | DateTime | The date to get working hours for. |

### Return Value

Working hours at the specified date.

### See Also

* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


