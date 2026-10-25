---
title: "ICalendar.GetWorkingTimes"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ICalendar. Επιστρέφει WorkingTimeCollection των εργάσιμων χρόνων για την καθορισμένη ημερομηνία"
type: docs
weight: 80
url: /el/net/aspose.tasks/icalendar/getworkingtimes/
---
## ICalendar.GetWorkingTimes method

Επιστρέφει [`WorkingTimeCollection`](../../workingtimecollection/) των εργάσιμων χρόνων για την καθορισμένη ημερομηνία.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dt | DateTime | Η ημερομηνία για την οποία θα ληφθούν οι ώρες εργασίας. |

### Τιμή Επιστροφής

Συλλογή αντικειμένων [`WorkingTime`](../../workingtime/).

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τη μέθοδο Calendar.GetIntersectionCalendar() για να εκτελέσετε υπολογισμό στο ημερολόγιο της ανάθεσης.

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

### Δείτε επίσης

* class [WorkingTimeCollection](../../workingtimecollection/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


