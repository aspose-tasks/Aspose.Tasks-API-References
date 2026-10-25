---
title: "Interfaz ICalendar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Interfaz Aspose.Tasks.ICalendar. Representa una abstracción de calendario que puede usarse para varios cálculos de fechas y duraciones."
type: docs
weight: 840
url: /es/net/aspose.tasks/icalendar/
---
## ICalendar interface

Representa una abstracción de calendario que puede usarse para varios cálculos de fechas y duraciones.

```csharp
public interface ICalendar
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Calcula la fecha en la que el tiempo de trabajo especificado habrá transcurrido según el calendario. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Calcula la fecha en la que el tiempo de trabajo especificado habrá transcurrido según el calendario. |
| [GetNextWorkingDayStart](../../aspose.tasks/icalendar/getnextworkingdaystart/)(DateTime) | Calcula el inicio del siguiente día laborable para la fecha especificada. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/icalendar/getpreviousworkingdayend/)(DateTime) | Calcula el final del día laborable anterior a partir de la fecha especificada. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Devuelve la fecha de inicio basada en la fecha de finalización y la duración especificadas. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Devuelve la fecha de inicio basada en la fecha de finalización y la duración especificadas. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/icalendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Calcula la fecha y hora de finalización de la tarea a partir de su fecha de inicio, sus partes divididas y la duración del trabajo. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours_1)(DateTime) | Devuelve la cantidad de horas laborables en la fecha especificada. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Devuelve WorkUnit - Inicio, Fin y Duración de las horas laborables para el intervalo de fecha y hora especificado. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/icalendar/getworkinghourstimespan/)(DateTime, DateTime) | Devuelve la cantidad de horas laborables entre las fechas especificadas. |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | Devuelve [`WorkingTimeCollection`](../workingtimecollection/) de tiempos laborables para la fecha especificada. |
| [GetWorkStart](../../aspose.tasks/icalendar/getworkstart/)(DateTime) | Calcula el inicio del siguiente tiempo laborable a partir de la fecha y hora especificadas. |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | Determina si el día especificado es un día laborable según el calendario. |
| [IsEmpty](../../aspose.tasks/icalendar/isempty/)() | Devuelve si el calendario no tiene horas laborables definidas. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


