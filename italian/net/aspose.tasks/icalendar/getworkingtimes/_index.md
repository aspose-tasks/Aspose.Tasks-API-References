---
title: "ICalendar.GetWorkingTimes"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ICalendar. Restituisce WorkingTimeCollection dei periodi lavorativi per la data specificata."
type: docs
weight: 80
url: /it/net/aspose.tasks/icalendar/getworkingtimes/
---
## ICalendar.GetWorkingTimes method

Restituisce [`WorkingTimeCollection`](../../workingtimecollection/) dei periodi lavorativi per la data specificata.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dt | DateTime | La data per cui ottenere gli orari di lavoro. |

### Valore di ritorno

Collezione di istanze di [`WorkingTime`](../../workingtime/).

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

* class [WorkingTimeCollection](../../workingtimecollection/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


