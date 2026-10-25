---
title: "WeekDay.SetDefaultWorkingTime"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "WeekDay метод. Устанавливает периоды времени по умолчанию для указанного дня недели."
type: docs
weight: 130
url: /ru/net/aspose.tasks/weekday/setdefaultworkingtime/
---
## WeekDay.SetDefaultWorkingTime method

Устанавливает периоды времени по умолчанию для указанного дня недели.

```csharp
public static void SetDefaultWorkingTime(WeekDay day)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| день | WeekDay | День недели, для которого устанавливается рабочий день по умолчанию. |

## Примеры

Показывает, как установить рабочее время по умолчанию для дня.

```csharp
var project = new Project();

// Определить календарь
var calendar = project.Calendars.Add("Calendar1");
calendar.WeekDays.Clear();

// Добавить рабочие дни с понедельника по четверг со стандартными часами
var monday = new WeekDay(DayType.Monday);
WeekDay.SetDefaultWorkingTime(monday);
calendar.WeekDays.Add(monday);
var tuesday = new WeekDay(DayType.Tuesday);
WeekDay.SetDefaultWorkingTime(tuesday);
calendar.WeekDays.Add(tuesday);
var wednesday = new WeekDay(DayType.Wednesday);
WeekDay.SetDefaultWorkingTime(wednesday);
calendar.WeekDays.Add(wednesday);
var thursday = new WeekDay(DayType.Thursday);
WeekDay.SetDefaultWorkingTime(thursday);
calendar.WeekDays.Add(thursday);
var friday = new WeekDay(DayType.Friday);
WeekDay.SetDefaultWorkingTime(friday);
calendar.WeekDays.Add(friday);

var saturday = new WeekDay(DayType.Saturday);
saturday.DayWorking = false;
calendar.WeekDays.Add(saturday);
var sunday = new WeekDay(DayType.Sunday);
sunday.DayWorking = false;
calendar.WeekDays.Add(sunday);

// выведем все рабочие времена
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### См. также

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


