---
title: "Calendar.GetIntersectionCalendar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Calendar. Obtiene una instancia ICalendar que puede usarse para realizar cálculos sobre la intersección de los horarios de trabajo de 2 calendarios"
type: docs
weight: 280
url: /es/net/aspose.tasks/calendar/getintersectioncalendar/
---
## Calendar.GetIntersectionCalendar method

Obtiene la instancia [`ICalendar`](../../icalendar/) que puede usarse para realizar cálculos sobre la intersección de los horarios de trabajo de 2 calendarios.

```csharp
public static ICalendar GetIntersectionCalendar(Calendar calendar1, Calendar calendar2)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| calendar1 | Calendar | Primer calendario. |
| calendar2 | Calendar | Segundo calendario. |

### Valor devuelto

Implementación de la interfaz ICalendar.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | Cuando cualquiera de los argumentos es nulo. |

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

* interface [ICalendar](../../icalendar/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


