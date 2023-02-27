---
title: Class Calendar
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Aspose.Tasks.Calendar clase. Representa un calendario utilizado en un proyecto.
type: docs
weight: 230
url: /es/net/aspose.tasks/calendar/
---
## Calendar class

Representa un calendario utilizado en un proyecto.

```csharp
public class Calendar
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | Obtiene o establece el calendario base del que depende este calendario. Solo aplicable si el calendario no es un calendario base. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | Obtiene el objeto CalendarExceptionCollection. La colección de excepciones que está asociada con el calendario. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | Obtiene un valor que indica si el calendario es un calendario base. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | Obtiene o establece un valor que indica si el calendario es un calendario de referencia. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | Obtiene o establece el nombre del calendario. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | Obtiene o establece el identificador único del calendario. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | Obtiene WeekDaysCollection para este calendario. La colección de días de la semana que define el calendario. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | Obtiene el objeto WorkWeekCollections. La colección de semanas laborales que está asociada con el calendario. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | Hace que un calendario determinado sea un calendario de 24 horas. El calendario de 24 horas es un calendario en el que todos los días de la semana funcionan con horario de trabajo las 24 horas. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | Convierte un Calendario determinado en Turno Nocturno. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | Crea un calendario estándar predeterminado. |
| [Delete](../../aspose.tasks/calendar/delete/)() | Elimina el calendario del proyecto. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Calcula la fecha en la que pasará la cantidad especificada de tiempo de trabajo según el calendario. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Calcula la fecha en la que pasará la cantidad especificada de tiempo de trabajo según el calendario. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | Devuelve un código hash para la instancia de la clase. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | Calcula el inicio del siguiente día hábil a partir de la fecha. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | Calcula el fin de la fecha de trabajo anterior a partir de la fecha especificada. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Devuelve la fecha de inicio en función de la fecha de finalización y la duración especificadas. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Devuelve la fecha de inicio en función de la fecha de finalización y la duración especificadas. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Calcula la fecha y hora de finalización de la tarea a partir de su fecha de inicio, las partes divididas y la duración. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | Devuelve la cantidad de horas de trabajo en la fecha. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Devolver horas de trabajo para las fechas especificadas. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | Devoluciones[`WorkingTimeCollection`](../workingtimecollection/) de horas de trabajo para la fecha especificada. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | Determina si el día es laborable. |

### Observaciones

Los calendarios se utilizan para definir los tiempos laborales y no laborales estándar. Los proyectos deben tener un calendario base. Las tareas y los recursos pueden tener sus propios calendarios no base que se basan en un calendario base.

### Ejemplos

Cómo crear un calendario sencillo desde cero.

```csharp
[C#]
// crea un calendario vacio
Calendar calendar = new Calendar("New calendar");
// añade días laborables predeterminados (8 horas laborables de 9:00 a 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// crea un nuevo dia laborable nuevo
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Establece el tiempo de trabajo. Solo la parte de tiempo de DateTime es importante
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
' crear calendario vacio
Dim calendar As Calendar =  New Calendar("New calendar")
' agrega días hábiles predeterminados (8 horas hábiles de 9:00 a 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' crear nuevo nuevo dia laborable
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Establece el tiempo de trabajo. Solo la parte de tiempo de DateTime es importante
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
' agrega fin de semana
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### Ver también

* espacio de nombres [Aspose.Tasks](../../aspose.tasks/)
* asamblea [Aspose.Tasks](../../)


