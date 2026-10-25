---
title: "Calendar.Name"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Calendar. Получает или задает имя календаря."
type: docs
weight: 90
url: /ru/net/aspose.tasks/calendar/name/
---
## Calendar.Name property

Получает или задает название календаря.

```csharp
public string Name { get; set; }
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


