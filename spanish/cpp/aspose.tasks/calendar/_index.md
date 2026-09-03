---
title: "Clase Aspose::Tasks::Calendar"
linktitle: "Calendario"
articleTitle: "Calendario"
second_title: "Aspose.Tasks for C++"
description: "Representa un calendario usado en un proyecto."
type: docs
weight: 10
url: /es/cpp/aspose.tasks/calendar/
---

## Calendar class

**Inherits:** Aspose::Tasks::ICalendar

Representa un calendario usado en un proyecto.

Cómo crear un calendario simple desde cero.

```cpp
[C#]
// crear calendario vacío
Calendar calendar = new Calendar("New calendar");
// agrega días laborables predeterminados (8 horas laborables de 9:00 a 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// crear nuevo día laborable
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Establece el tiempo de trabajo. Solo la parte de hora de DateTime es importante.
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

```cpp
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

Los calendarios se utilizan para definir horarios estándar de trabajo y no trabajo. Los proyectos deben tener un calendario base. Las tareas y los recursos pueden tener sus propios calendarios no base que se basan en un calendario base.

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Delete](./delete/) | Elimina el calendario del proyecto. |
| [Equals](./equals/) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [get_BaseCalendar](./get_basecalendar/) | Obtiene el calendario base del cual depende este calendario. Solo aplicable si el calendario no es un calendario base. |
| [get_Exceptions](./get_exceptions/) | Obtiene el objeto CalendarExceptionCollection. La colección de excepciones asociada al calendario. |
| [get_Guid](./get_guid/) | Obtiene el GUID del calendario. |
| [get_IsBaseCalendar](./get_isbasecalendar/) | Obtiene un valor que indica si el calendario es un calendario base. |
| [get_IsBaselineCalendar](./get_isbaselinecalendar/) | Obtiene un valor que indica si el calendario es un calendario de referencia. |
| [get_Name](./get_name/) | Obtiene el nombre del calendario. |
| [get_Uid](./get_uid/) | Obtiene el identificador único del calendario. |
| [get_WeekDays](./get_weekdays/) | Obtiene WeekDaysCollection para este calendario. La colección de días de la semana que define el calendario. |
| [get_WorkWeeks](./get_workweeks/) | Obtiene el objeto WorkWeekCollections. La colección de semanas laborales asociada al calendario. |
| [GetFinishDateByStartAndWork (2 overloads)](./getfinishdatebystartandwork/) | Calcula la fecha en la que el tiempo de trabajo especificado habrá transcurrido según el calendario. |
| [GetHashCode](./gethashcode/) | Devuelve un código hash para la instancia de la clase. |
| [GetIntersectionCalendar](./getintersectioncalendar/) | Obtiene la instancia ICalendar que puede usarse para realizar cálculos sobre la intersección de horarios de trabajo de 2 calendarios. |
| [GetNextWorkingDayStart](./getnextworkingdaystart/) | Calcula el inicio del siguiente día laborable para la fecha especificada. |
| [GetPreviousWorkingDayEnd](./getpreviousworkingdayend/) | Calcula el final de la fecha laborable anterior a partir de la fecha especificada. |
| [GetStartDateFromFinishAndDuration (2 overloads)](./getstartdatefromfinishandduration/) | Devuelve la fecha de inicio basada en la fecha de finalización y la duración especificadas. |
| [GetTaskFinishDateFromDuration](./gettaskfinishdatefromduration/) | Calcula la fecha y hora de finalización de la tarea a partir de su fecha de inicio, partes divididas y la duración del trabajo. |
| [GetWorkingHours (2 overloads)](./getworkinghours/) | Devuelve la cantidad de horas laborables en la fecha especificada. |
| [GetWorkingHoursTimeSpan](./getworkinghourstimespan/) | Devuelve la cantidad de horas laborables entre las fechas especificadas. |
| [GetWorkingTimes](./getworkingtimes/) | Devuelve WorkingTimeCollection de tiempos laborables para la fecha especificada. |
| [GetWorkStart](./getworkstart/) | Calcula el inicio del siguiente tiempo laborable a partir de la fecha y hora especificadas. |
| [IsDayWorking](./isdayworking/) | Determina si el día especificado es un día laborable según el calendario. |
| [IsEmpty](./isempty/) | Devuelve si el calendario no tiene horas laborables definidas. |
| [Make24HourCalendar](./make24hourcalendar/) | Convierte un calendario dado en un Calendario de 24 Horas. El Calendario de 24 Horas es un calendario en el que cada día de la semana trabaja con horario continuo. |
| [MakeNightShiftCalendar](./makenightshiftcalendar/) | Convierte un calendario dado en un Calendario de Turno Nocturno. |
| [MakeStandardCalendar](./makestandardcalendar/) | Crea un calendario estándar predeterminado. |
| [set_BaseCalendar](./set_basecalendar/) | Establece el calendario base del cual depende este calendario. Solo aplicable si el calendario no es un calendario base. |
| [set_IsBaselineCalendar](./set_isbaselinecalendar/) | Establece un valor que indica si el calendario es un calendario de referencia. |
| [set_Name](./set_name/) | Establece el nombre del calendario. |
| [set_Uid](./set_uid/) | Establece el identificador único del calendario. |

