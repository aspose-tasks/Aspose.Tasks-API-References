---
title: "Класс Calendar"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Calendar. Представляет календарь, используемый в проекте."
type: docs
weight: 230
url: /ru/net/aspose.tasks/calendar/
---
## Calendar class

Представляет календарь, используемый в проекте.

```csharp
public class Calendar : ICalendar
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | Получает или задает базовый календарь, от которого зависит этот календарь. Применяется только если календарь не является базовым. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | Получает объект CalendarExceptionCollection. Коллекция исключений, связанных с календарем. |
| [Guid](../../aspose.tasks/calendar/guid/) { get; } | Получает GUID календаря. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | Получает значение, указывающее, является ли календарь базовым. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | Получает или задает значение, указывающее, является ли календарь базовым календарем. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | Получает или задает название календаря. |
| [PrimaveraProperties](../../aspose.tasks/calendar/primaveraproperties/) { get; } | Получает объект, содержащий свойства, специфичные для Primavera, для календаря, считанного из форматов Primavera. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | Получает или задает уникальный идентификатор календаря. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | Получает WeekDaysCollection для этого календаря. Коллекция дней недели, определяющих календарь. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | Получает объект WorkWeekCollections. Коллекция рабочих недель, связанных с календарем. |

## Методы

| Имя | Описание |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | Превращает заданный Calendar в 24‑часовой календарь. 24‑часовой календарь — это календарь, в котором каждый день недели работает круглосуточно. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | Создает указанный календарь как календарь ночной смены. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | Создает стандартный календарь по умолчанию. |
| [Delete](../../aspose.tasks/calendar/delete/)() | Удаляет календарь из проекта. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Вычисляет дату, когда указанное количество рабочего времени пройдет согласно календарю. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Вычисляет дату, когда указанное количество рабочего времени пройдет согласно календарю. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | Возвращает хеш‑код для экземпляра класса. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | Вычисляет начало следующего рабочего дня для указанной даты. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | Вычисляет конец предыдущего рабочего дня относительно указанной даты. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Возвращает дату начала, исходя из указанной даты завершения и длительности. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Возвращает дату начала, исходя из указанной даты завершения и длительности. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Вычисляет дату и время завершения задачи на основе её даты начала, разбитых частей и длительности работы. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | Возвращает количество рабочих часов на указанную дату. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Возвращает WorkUnit — начало, конец и продолжительность рабочих часов для указанного интервала даты и времени. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/calendar/getworkinghourstimespan/)(DateTime, DateTime) | Возвращает количество рабочих часов между указанными датами. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | Возвращает [`WorkingTimeCollection`](../workingtimecollection/) рабочих периодов для указанной даты. |
| [GetWorkStart](../../aspose.tasks/calendar/getworkstart/)(DateTime) | Вычисляет начало следующего рабочего периода, начиная с указанной даты и времени. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | Определяет, является ли указанный день рабочим согласно календарю. |
| virtual [IsEmpty](../../aspose.tasks/calendar/isempty/)() | Возвращает, определено ли в календаре отсутствие рабочих часов. |
| static [GetIntersectionCalendar](../../aspose.tasks/calendar/getintersectioncalendar/)(Calendar, Calendar) | Получает экземпляр [`ICalendar`](../icalendar/), который можно использовать для выполнения вычислений пересечения графиков работы двух календарей. |

## Примечания

Календари используются для определения стандартных рабочих и нерабочих периодов. Проекты должны иметь один базовый календарь. Задачи и ресурсы могут иметь свои собственные небазовые календари, основанные на базовом календаре.

## Примеры

Как создать простой календарь с нуля.

```csharp
[C#]
// создать пустой календарь
Calendar calendar = new Calendar("New calendar");
// добавляет стандартные рабочие дни (8 рабочих часов с 9:00 до 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// создать новый рабочий день
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Устанавливает рабочее время. Важна только часть времени объекта DateTime.
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
// добавляет выходные
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

Показывает, как определить новый календарь, добавить к нему будние дни и задать рабочие часы для дней.

```csharp
var project = new Project();

// Определить календарь
var calendar = project.Calendars.Add("Calendar1");

// Добавить рабочие дни с понедельника по четверг со стандартными часами
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Установить пятницу как короткий рабочий день
var weekDay = new WeekDay(DayType.Friday);

// Устанавливает рабочее время. Важна только часть времени объекта DateTime.
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// работа с проектом...
```

### См. также

* interface [ICalendar](../icalendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


