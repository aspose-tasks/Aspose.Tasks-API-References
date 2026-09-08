---
title: "ICalendar.GetWorkingHours"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ICalendar. Devuelve WorkUnit Inicio, Fin y Duración de las horas de trabajo para el intervalo de fecha y hora especificado."
type: docs
weight: 60
url: /es/net/aspose.tasks/icalendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Devuelve WorkUnit - Inicio, Fin y Duración de las horas laborables para el intervalo de fecha y hora especificado.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | DateTime | Fecha de inicio del intervalo. |
| finalizar | DateTime | Fecha de finalización del intervalo. |

### Valor devuelto

Instancia de la clase [`WorkUnit`](../../workunit/) que contiene Inicio, Fin y Duración de las horas de trabajo.

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

* class [WorkUnit](../../workunit/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Devuelve la cantidad de horas laborables en la fecha especificada.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dt | DateTime | La fecha para la que se obtienen las horas de trabajo. |

### Valor devuelto

Horas de trabajo en la fecha especificada.

### Ver también

* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


