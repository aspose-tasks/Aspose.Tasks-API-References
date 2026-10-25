---
title: "ICalendar.GetWorkingHours"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ICalendar. Restituisce WorkUnit Start Finish e Duration delle ore lavorative per l'intervallo di data e ora specificato."
type: docs
weight: 60
url: /it/net/aspose.tasks/icalendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Restituisce WorkUnit - Inizio, Fine e Durata delle ore lavorative per l'intervallo di data e ora specificato.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | DateTime | Data di inizio dell'intervallo. |
| fine | DateTime | Data di fine dell'intervallo. |

### Valore di ritorno

Istanza della classe [`WorkUnit`](../../workunit/) contenente Start, Finish e Duration delle ore lavorative.

## Esempi

Mostra come utilizzare il metodo Calendar.GetIntersectionCalendar() per eseguire il calcolo sul calendario dell'assegnazione.

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

### Vedi anche

* class [WorkUnit](../../workunit/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Restituisce la quantità di ore lavorative nella data specificata.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dt | DateTime | La data per cui ottenere le ore lavorative. |

### Valore di ritorno

Ore lavorative nella data specificata.

### Vedi anche

* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


