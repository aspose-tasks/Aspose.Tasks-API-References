---
title: "Calendar.IsBaselineCalendar"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Calendar. Возвращает или задает значение, указывающее, является ли календарь baseline calendar"
type: docs
weight: 80
url: /ru/net/aspose.tasks/calendar/isbaselinecalendar/
---
## Calendar.IsBaselineCalendar property

Получает или задает значение, указывающее, является ли календарь базовым календарем.

```csharp
public bool IsBaselineCalendar { get; set; }
```

## Примеры

Показывает, как проверить, является ли календарь baseline calendar или нет.

```csharp
var project = new Project(DataDir + "IsBaselineCalendar.mpp");

var calendar = project.Calendars.GetByUid(3);

Console.WriteLine("Is baseline calendar: " + calendar.IsBaselineCalendar);
```

### См. также

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


