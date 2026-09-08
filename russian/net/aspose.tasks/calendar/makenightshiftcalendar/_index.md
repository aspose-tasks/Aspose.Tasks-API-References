---
title: "Calendar.MakeNightShiftCalendar"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Calendar. Преобразует указанный Calendar в Night Shift Calendar"
type: docs
weight: 20
url: /ru/net/aspose.tasks/calendar/makenightshiftcalendar/
---
## Calendar.MakeNightShiftCalendar method

Создает указанный календарь как календарь ночной смены.

```csharp
public static Calendar MakeNightShiftCalendar(Calendar calendar)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| календарь | Calendar | Calendar для создания Night Shift Calendar. |

### Возвращаемое значение

Night Shift Calendar.

## Примеры

Показывает, как создать Night Shift Calendar.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// показать рабочие часы
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Показывает, как преобразовать календарь в Night Shift Calendar.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("Night Shift");
calendar = Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// показать рабочие часы
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

### См. также

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


