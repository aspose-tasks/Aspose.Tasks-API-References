---
title: "Calendar.GetIntersectionCalendar"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Calendar-Methode. Gibt eine ICalendar-Instanz zurück, die verwendet werden kann, um Berechnungen an der Schnittmenge von Arbeitsplänen zweier Kalender durchzuführen"
type: docs
weight: 280
url: /de/net/aspose.tasks/calendar/getintersectioncalendar/
---
## Calendar.GetIntersectionCalendar method

Gibt eine [`ICalendar`](../../icalendar/) Instanz zurück, die verwendet werden kann, um Berechnungen an der Schnittmenge von Arbeitsplänen zweier Kalender durchzuführen.

```csharp
public static ICalendar GetIntersectionCalendar(Calendar calendar1, Calendar calendar2)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| calendar1 | Calendar | Erster Kalender. |
| calendar2 | Calendar | Zweiter Kalender. |

### Rückgabewert

Implementierung des ICalendar-Interfaces.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Wenn eines der Argumente null ist. |

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

* interface [ICalendar](../../icalendar/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


