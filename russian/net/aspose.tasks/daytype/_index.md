---
title: "Перечисление DayType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.DayType enum. Указывает день недели"
type: docs
weight: 450
url: /ru/net/aspose.tasks/daytype/
---
## DayType enumeration

Указывает день недели.

```csharp
public enum DayType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Exception | `0` | Указывает тип дня Exception. |
| Sunday | `1` | Указывает тип дня Sunday. |
| Monday | `2` | Указывает тип дня Monday. |
| Tuesday | `3` | Указывает тип дня Tuesday. |
| Wednesday | `4` | Указывает тип дня Wednesday. |
| Thursday | `5` | Указывает тип дня Thursday. |
| Friday | `6` | Указывает тип дня Friday. |
| Saturday | `7` | Указывает тип дня Saturday. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


