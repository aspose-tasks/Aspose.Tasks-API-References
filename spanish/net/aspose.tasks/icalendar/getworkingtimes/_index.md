---
title: "ICalendar.GetWorkingTimes"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de ICalendar. Devuelve WorkingTimeCollection de tiempos laborables para la fecha especificada"
type: docs
weight: 80
url: /es/net/aspose.tasks/icalendar/getworkingtimes/
---
## ICalendar.GetWorkingTimes method

Devuelve [`WorkingTimeCollection`](../../workingtimecollection/) de tiempos laborables para la fecha especificada.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dt | DateTime | La fecha para la que se obtienen los tiempos de trabajo. |

### Valor devuelto

Colección de instancias de [`WorkingTime`](../../workingtime/).

## Ejemplos

Muestra cómo usar el método Calendar.GetIntersectionCalendar() para realizar cálculos en el calendario de la asignación.

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

### Ver también

* class [WorkingTimeCollection](../../workingtimecollection/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


