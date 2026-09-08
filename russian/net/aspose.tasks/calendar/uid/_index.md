---
title: "Calendar.Uid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Calendar. Получает или задает уникальный идентификатор календаря"
type: docs
weight: 110
url: /ru/net/aspose.tasks/calendar/uid/
---
## Calendar.Uid property

Получает или задает уникальный идентификатор календаря.

```csharp
public int Uid { get; set; }
```

## Примеры

Показывает, как получить информацию о календаре.

```csharp
var project = new Project(DataDir + "RetrieveCalendarInfo.mpp");

// Получить информацию о календарях
foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("Calendar UID: " + calendar.Uid);
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### См. также

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


