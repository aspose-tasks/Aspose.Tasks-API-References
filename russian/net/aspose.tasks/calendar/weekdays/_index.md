---
title: "Calendar.WeekDays"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Calendar. Возвращает WeekDaysCollection для этого календаря. Коллекция дней недели, определяющих календарь."
type: docs
weight: 120
url: /ru/net/aspose.tasks/calendar/weekdays/
---
## Calendar.WeekDays property

Получает WeekDaysCollection для этого календаря. Коллекция дней недели, определяющих календарь.

```csharp
public WeekDayCollection WeekDays { get; }
```

## Примеры

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

* class [WeekDayCollection](../../weekdaycollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


