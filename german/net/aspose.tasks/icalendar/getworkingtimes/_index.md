---
title: "ICalendar.GetWorkingTimes"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "ICalendar-Methode. Gibt eine WorkingTimeCollection von Arbeitszeiten für das angegebene Datum zurück."
type: docs
weight: 80
url: /de/net/aspose.tasks/icalendar/getworkingtimes/
---
## ICalendar.GetWorkingTimes method

Gibt [`WorkingTimeCollection`](../../workingtimecollection/) von Arbeitszeiten für das angegebene Datum zurück.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dt | DateTime | Das Datum, für das die Arbeitszeiten abgerufen werden sollen. |

### Rückgabewert

Sammlung von [`WorkingTime`](../../workingtime/)-Instanzen.

## Beispiele

Zeigt, wie die Methode Calendar.GetIntersectionCalendar() verwendet wird, um Berechnungen im Kalender der Zuordnung durchzuführen.

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

### Siehe auch

* class [WorkingTimeCollection](../../workingtimecollection/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


