---
title: "класс Aspose::Tasks::Calendar"
linktitle: "Календарь"
articleTitle: "Календарь"
second_title: "Aspose.Tasks для C++"
description: "Представляет календарь, используемый в проекте."
type: docs
weight: 10
url: /ru/cpp/aspose.tasks/calendar/
---

## Calendar class

**Inherits:** Aspose::Tasks::ICalendar

Представляет календарь, используемый в проекте.

Как создать простой календарь с нуля.

```cpp
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

Календари используются для определения стандартных рабочих и нерабочих периодов. У проектов должен быть один базовый календарь. Задачи и ресурсы могут иметь свои собственные небазовые календари, которые основаны на базовом календаре.

## Методы

| Имя | Описание |
| --- | --- |
| [Delete](./delete/) | Удаляет календарь из проекта. |
| [Equals](./equals/) | Возвращает значение, указывающее, равен ли этот экземпляр заданному объекту. |
| [get_BaseCalendar](./get_basecalendar/) | Получает базовый календарь, от которого зависит этот календарь. Применяется только если календарь не является базовым календарём. |
| [get_Exceptions](./get_exceptions/) | Получает объект CalendarExceptionCollection. Коллекция исключений, связанная с календарём. |
| [get_Guid](./get_guid/) | Получает Guid календаря. |
| [get_IsBaseCalendar](./get_isbasecalendar/) | Получает значение, указывающее, является ли календарь базовым. |
| [get_IsBaselineCalendar](./get_isbaselinecalendar/) | Получает значение, указывающее, является ли календарь исходным календарём. |
| [get_Name](./get_name/) | Получает имя календаря. |
| [get_Uid](./get_uid/) | Получает уникальный идентификатор календаря. |
| [get_WeekDays](./get_weekdays/) | Получает WeekDaysCollection для этого календаря. Коллекция дней недели, определяющая календарь. |
| [get_WorkWeeks](./get_workweeks/) | Получает объект WorkWeekCollections. Коллекция рабочих недель, связанная с календарём. |
| [GetFinishDateByStartAndWork (2 overloads)](./getfinishdatebystartandwork/) | Вычисляет дату, когда указанное количество рабочего времени пройдет согласно календарю. |
| [GetHashCode](./gethashcode/) | Возвращает хеш‑код экземпляра класса. |
| [GetIntersectionCalendar](./getintersectioncalendar/) | Получает экземпляр ICalendar, который можно использовать для вычислений пересечения рабочих расписаний двух календарей. |
| [GetNextWorkingDayStart](./getnextworkingdaystart/) | Вычисляет начало следующего рабочего дня для указанной даты. |
| [GetPreviousWorkingDayEnd](./getpreviousworkingdayend/) | Вычисляет конец предыдущей рабочей даты относительно указанной даты. |
| [GetStartDateFromFinishAndDuration (2 overloads)](./getstartdatefromfinishandduration/) | Возвращает дату начала на основе указанной даты завершения и длительности. |
| [GetTaskFinishDateFromDuration](./gettaskfinishdatefromduration/) | Вычисляет дату и время завершения задачи исходя из её даты начала, разбитых частей и длительности работы. |
| [GetWorkingHours (2 overloads)](./getworkinghours/) | Возвращает количество рабочих часов на указанную дату. |
| [GetWorkingHoursTimeSpan](./getworkinghourstimespan/) | Возвращает количество рабочих часов между указанными датами. |
| [GetWorkingTimes](./getworkingtimes/) | Возвращает WorkingTimeCollection рабочих времён для указанной даты. |
| [GetWorkStart](./getworkstart/) | Вычисляет начало следующего рабочего времени, начиная с указанной даты и времени. |
| [IsDayWorking](./isdayworking/) | Определяет, является ли указанный день рабочим согласно календарю. |
| [IsEmpty](./isempty/) | Возвращает, не определены ли в календаре рабочие часы. |
| [Make24HourCalendar](./make24hourcalendar/) | Преобразует указанный календарь в 24‑часовой календарь. 24‑часовой календарь — это календарь, в котором каждый день недели работает круглосуточно. |
| [MakeNightShiftCalendar](./makenightshiftcalendar/) | Преобразует указанный календарь в Night Shift Calendar. |
| [MakeStandardCalendar](./makestandardcalendar/) | Создаёт стандартный календарь по умолчанию. |
| [set_BaseCalendar](./set_basecalendar/) | Устанавливает базовый календарь, от которого зависит этот календарь. Применяется только если календарь не является базовым. |
| [set_IsBaselineCalendar](./set_isbaselinecalendar/) | Устанавливает значение, указывающее, является ли календарь исходным календарём. |
| [set_Name](./set_name/) | Устанавливает имя календаря. |
| [set_Uid](./set_uid/) | Устанавливает уникальный идентификатор календаря. |

