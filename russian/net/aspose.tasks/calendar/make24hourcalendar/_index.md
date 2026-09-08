---
title: "Calendar.Make24HourCalendar"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Calendar. Преобразует заданный календарь в 24‑часовой календарь. 24‑часовой календарь — это календарь, в котором каждый день недели работает круглосуточно."
type: docs
weight: 10
url: /ru/net/aspose.tasks/calendar/make24hourcalendar/
---
## Calendar.Make24HourCalendar method

Превращает заданный Calendar в 24‑часовой календарь. 24‑часовой календарь — это календарь, в котором каждый день недели работает круглосуточно.

```csharp
public static Calendar Make24HourCalendar(Calendar calendar)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| календарь | Calendar | Календарь для создания 24‑часового календаря из. |

### Возвращаемое значение

Календарь 24‑часовой.

## Примеры

Показывает, как создать 24‑часовой календарь.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// Будут выведены 24 часа
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

Показывает, как преобразовать новый календарь в 24‑часовой календарь.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("24 Hours");
calendar = Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// Будут выведены 24 часа
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

### См. также

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


