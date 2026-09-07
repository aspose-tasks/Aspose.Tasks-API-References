---
title: "ICalendar.GetWorkingHours"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "ICalendar-Methode. Gibt WorkUnit Start, Finish und Duration der Arbeitsstunden für das angegebene Datums‑Zeitintervall zurück."
type: docs
weight: 60
url: /de/net/aspose.tasks/icalendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Gibt WorkUnit – Start, Ende und Dauer der Arbeitsstunden für das angegebene Datums‑Zeitintervall zurück.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Start | DateTime | Startdatum des Intervalls. |
| Ende | DateTime | Enddatum des Intervalls. |

### Rückgabewert

Instanz der Klasse [`WorkUnit`](../../workunit/), die Start, Finish und Duration der Arbeitsstunden enthält.

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

* class [WorkUnit](../../workunit/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Gibt die Anzahl der Arbeitsstunden am angegebenen Datum zurück.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dt | DateTime | Das Datum, für das die Arbeitsstunden abgerufen werden sollen. |

### Rückgabewert

Arbeitsstunden am angegebenen Datum.

### Siehe auch

* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


