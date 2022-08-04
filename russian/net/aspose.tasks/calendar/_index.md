---
title: Calendar
second_title: Справочник по Aspose.Tasks для .NET API
description: Представляет календарь используемый в проекте.
type: docs
weight: 220
url: /ru/net/aspose.tasks/calendar/
---
## Calendar class

Представляет календарь, используемый в проекте.

```csharp
public class Calendar
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar) { get; set; } | Получает или задает базовый календарь, от которого зависит этот календарь. Применяется только в том случае, если календарь не является базовым. Чтение/запись[`Calendar`](../calendar) . |
| [Exceptions](../../aspose.tasks/calendar/exceptions) { get; } | Получает объект CalendarExceptionCollection. Коллекция исключений, связанных с календарем. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar) { get; } | Получает значение, указывающее, является ли календарь базовым. Только для чтенияBoolean . |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar) { get; set; } | Получает или задает значение, указывающее, является ли календарь базовым календарем. Чтение/записьBoolean . |
| [Name](../../aspose.tasks/calendar/name) { get; set; } | Получает или задает имя календаря. Чтение/записьString . |
| [ParentProject](../../aspose.tasks/calendar/parentproject) { get; } | Получает родительский проект для этого календаря. |
| [Uid](../../aspose.tasks/calendar/uid) { get; set; } | Получает или задает уникальный идентификатор календаря. Чтение/записьInt32 . |
| [WeekDays](../../aspose.tasks/calendar/weekdays) { get; } | Получает WeekDaysCollection для этого календаря. Коллекция дней недели, которая определяет календарь. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks) { get; } | Получает объект WorkWeekCollections. Коллекция рабочих недель, связанная с календарем. |

## Методы

| Имя | Описание |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar)(Calendar) | Делает данный календарь 24-часовым календарем. 24-часовой календарь — это календарь, в котором каждый день недели работает с круглосуточным рабочим временем. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar)(Calendar) | Делает данный календарь календарем ночной смены. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar)(Calendar) | Создает стандартный календарь по умолчанию. |
| [Delete](../../aspose.tasks/calendar/delete)() | Удаляет календарь из проекта. |
| override [Equals](../../aspose.tasks/calendar/equals)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork#getfinishdatebystartandwork)(DateTime, Duration) | Вычисляет дату, когда пройдет указанное количество рабочего времени по календарю. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Вычисляет дату, когда пройдет указанное количество рабочего времени по календарю. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode)() | Возвращает хэш-код экземпляра[`Calendar`](../calendar) класс. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart)(DateTime) | Рассчитывает начало следующего рабочего дня с даты. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend)(DateTime) | Вычисляет конец предыдущей рабочей даты от указанной даты. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration#getstartdatefromfinishandduration)(DateTime, Duration) | Возвращает StartDate на основе указанных FinishDate и Duration. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Возвращает StartDate на основе указанных FinishDate и Duration. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration)(Task, TimeSpan) | Вычисляет дату и время окончания задачи, исходя из даты ее начала, разделенных частей и продолжительности. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours#getworkinghours_1)(DateTime) | Возвращает количество рабочих часов на дату. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours#getworkinghours)(DateTime, DateTime) | Возврат рабочего времени для указанных дат. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes)(DateTime) | Возвращает[`WorkingTimeCollection`](../workingtimecollection) рабочего времени. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking)(DateTime) | Определяет, является ли день рабочим. |

### Примечания

Календари используются для определения стандартного рабочего и нерабочего времени. Проекты должны иметь один базовый календарь. Задачи и ресурсы могут иметь собственные небазовые календари, основанные на базовом календаре.

### Примеры

Как создать простой календарь с нуля.

```csharp
[C#]
// создаем пустой календарь
Calendar calendar = new Calendar("New calendar");
// добавляем рабочие дни по умолчанию (8 рабочих часов с 9:00 до 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// создаем новый новый рабочий день
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Устанавливает рабочее время. Важна только временная часть DateTime
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
// добавляем выходные
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' создать пустой календарь
Dim calendar As Calendar =  New Calendar("New calendar")
' добавляет рабочие дни по умолчанию (8 рабочих часов с 9:00 до 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' создать новый новый рабочий день
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Устанавливает рабочее время. Важна только временная часть DateTime
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
' добавляет выходные
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### Смотрите также

* пространство имен [Aspose.Tasks](../../aspose.tasks)
* сборка [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
