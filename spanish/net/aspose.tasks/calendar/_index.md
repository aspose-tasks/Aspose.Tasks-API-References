---
title: "Clase Calendar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Calendar. Representa un calendario utilizado en un proyecto"
type: docs
weight: 230
url: /es/net/aspose.tasks/calendar/
---
## Calendar class

Representa un calendario usado en un proyecto.

```csharp
public class Calendar : ICalendar
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | Obtiene o establece el calendario base del cual depende este calendario. Solo aplicable si el calendario no es un calendario base. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | Obtiene el objeto CalendarExceptionCollection. La colección de excepciones asociada al calendario. |
| [Guid](../../aspose.tasks/calendar/guid/) { get; } | Obtiene el Guid del calendario. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | Obtiene un valor que indica si el calendario es un calendario base. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | Obtiene o establece un valor que indica si el calendario es un calendario de línea base. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | Obtiene o establece el nombre del calendario. |
| [PrimaveraProperties](../../aspose.tasks/calendar/primaveraproperties/) { get; } | Obtiene un objeto que contiene propiedades específicas de Primavera para un calendario leído de formatos Primavera. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | Obtiene o establece el identificador único del calendario. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | Obtiene WeekDaysCollection para este calendario. La colección de días laborables que define el calendario. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | Obtiene el objeto WorkWeekCollections. La colección de semanas laborables asociada al calendario. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | Convierte un Calendar dado en un Calendar de 24 horas. El Calendar de 24 horas es un calendario en el que cada día de la semana trabaja con horarios continuos. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | Convierte un Calendar dado en un Calendar de turno nocturno. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | Crea un calendar estándar predeterminado. |
| [Delete](../../aspose.tasks/calendar/delete/)() | Elimina el calendar del proyecto. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Calcula la fecha en la que el tiempo de trabajo especificado habrá transcurrido según el calendario. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Calcula la fecha en la que el tiempo de trabajo especificado habrá transcurrido según el calendario. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | Devuelve un código hash para la instancia de la clase. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | Calcula el inicio del siguiente día laborable para la fecha especificada. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | Calcula el final del día laborable anterior a partir de la fecha especificada. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Devuelve la fecha de inicio basada en la fecha de finalización y la duración especificadas. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Devuelve la fecha de inicio basada en la fecha de finalización y la duración especificadas. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Calcula la fecha y hora de finalización de la tarea a partir de su fecha de inicio, sus partes divididas y la duración del trabajo. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | Devuelve la cantidad de horas laborables en la fecha especificada. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Devuelve WorkUnit - Inicio, Fin y Duración de las horas de trabajo para el intervalo de fecha y hora especificado. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/calendar/getworkinghourstimespan/)(DateTime, DateTime) | Devuelve la cantidad de horas laborables entre las fechas especificadas. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | Devuelve [`WorkingTimeCollection`](../workingtimecollection/) de tiempos laborables para la fecha especificada. |
| [GetWorkStart](../../aspose.tasks/calendar/getworkstart/)(DateTime) | Calcula el inicio del siguiente tiempo laborable a partir de la fecha y hora especificadas. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | Determina si el día especificado es un día laborable según el calendario. |
| virtual [IsEmpty](../../aspose.tasks/calendar/isempty/)() | Devuelve si el calendario no tiene horas laborables definidas. |
| static [GetIntersectionCalendar](../../aspose.tasks/calendar/getintersectioncalendar/)(Calendar, Calendar) | Obtiene la instancia [`ICalendar`](../icalendar/) que puede usarse para realizar cálculos sobre la intersección de los horarios de trabajo de 2 calendars. |

## Observaciones

Los calendars se utilizan para definir los tiempos de trabajo y no trabajo estándar. Los proyectos deben tener un calendar base. Las tareas y los recursos pueden tener sus propios calendars no base que se basan en un calendar base.

## Ejemplos

Cómo crear un calendar simple desde cero.

```csharp
[C#]
// crear calendar vacío
Calendar calendar = new Calendar("New calendar");
// agrega días laborables predeterminados (8 horas de trabajo de 9:00 a 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// crear nuevo día laborable
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Establece el tiempo de trabajo. Solo la parte de hora de `DateTime` es importante
    WorkingTime wt1 = new WorkingTime();
    wt1.FromTime = new DateTime(1, 1, 1, 6, 0, 0, 0);
    wt1.ToTime = new DateTime(1, 1, 1, 12, 0, 0, 0);
    WorkingTime wt2 = new WorkingTime();
    wt2.FromTime = new DateTime(1, 1, 1, 14, 0, 0, 0);
    wt2.ToTime = new DateTime(1, 1, 1, 18, 0, 0, 0);
    myWeekDay.WorkingTimes.Add(wt1);
    myWeekDay.WorkingTimes.Add(wt2);
    myWeekDay.DayWorking = true;
calendar.Days.Add(myWeekDay);
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
// agrega fin de semana
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' create empty calendar
Dim calendar As Calendar =  New Calendar("New calendar")
' adds default working days (8 working hours from 9:00 to 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' create new new working day
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Sets working time. Only time part of DateTime is important
    Dim wt1 As WorkingTime =  New WorkingTime()
    wt1.FromTime = New DateTime(1, 1, 1, 6, 0, 0, 0)
    wt1.ToTime = New DateTime(1, 1, 1, 12, 0, 0, 0)
    Dim wt2 As WorkingTime =  New WorkingTime()
    wt2.FromTime = New DateTime(1, 1, 1, 14, 0, 0, 0)
    wt2.ToTime = New DateTime(1, 1, 1, 18, 0, 0, 0)
    myWeekDay.WorkingTimes.Add(wt1)
    myWeekDay.WorkingTimes.Add(wt2)
    myWeekDay.DayWorking = True
calendar.Days.Add(myWeekDay)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday))
' adds weekend
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

Muestra cómo definir un calendar nuevo, agregar días de la semana a él y definir los horarios de trabajo para los días.

```csharp
var project = new Project();

// Definir un calendar
var calendar = project.Calendars.Add("Calendar1");

// Agregar días laborables de lunes a jueves con horarios predeterminados
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Establecer el viernes como día laborable corto
var weekDay = new WeekDay(DayType.Friday);

// Establece el tiempo de trabajo. Solo la parte de hora de `DateTime` es importante
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// trabajando con el proyecto...
```

### Ver también

* interface [ICalendar](../icalendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


