---
title: "ICalendar.GetWorkingHours"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ICalendar-methode. Retourneert WorkUnit Start, Finish en Duration van werktijd voor het opgegeven datum‑tijdinterval."
type: docs
weight: 60
url: /nl/net/aspose.tasks/icalendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Retourneert WorkUnit - Start, Eind en Duur van werkuren voor het opgegeven datum-tijdinterval.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | DateTime | Startdatum van het interval. |
| einde | DateTime | Einddatum van het interval. |

### Retourwaarde

Instantie van de [`WorkUnit`](../../workunit/) klasse die Start, Finish en Duration van werktijd bevat.

## Voorbeelden

Toont hoe de methode Calendar.GetIntersectionCalendar() te gebruiken om berekeningen uit te voeren op de kalender van de toewijzing.

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

### Zie ook

* class [WorkUnit](../../workunit/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Retourneert het aantal werkuren op de opgegeven datum.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dt | DateTime | De datum om werktijden voor op te halen. |

### Retourwaarde

Werktijden op de opgegeven datum.

### Zie ook

* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


