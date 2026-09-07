---
title: "Calendar.GetIntersectionCalendar"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Calendar. Ottiene un'istanza ICalendar che può essere usata per eseguire calcoli sull'intersezione degli orari di lavoro di 2 calendari"
type: docs
weight: 280
url: /it/net/aspose.tasks/calendar/getintersectioncalendar/
---
## Calendar.GetIntersectionCalendar method

Ottiene l'istanza [`ICalendar`](../../icalendar/) che può essere usata per eseguire calcoli sull'intersezione degli orari di lavoro di 2 calendari.

```csharp
public static ICalendar GetIntersectionCalendar(Calendar calendar1, Calendar calendar2)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| calendar1 | Calendar | Primo calendario. |
| calendar2 | Calendar | Secondo calendario. |

### Valore di ritorno

Implementazione dell'interfaccia ICalendar.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Quando uno qualsiasi degli argomenti è nullo. |

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

* interface [ICalendar](../../icalendar/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


