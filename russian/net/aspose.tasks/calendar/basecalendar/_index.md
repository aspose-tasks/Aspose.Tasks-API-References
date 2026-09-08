---
title: "Calendar.BaseCalendar"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Calendar. Получает или задает базовый календарь, от которого зависит данный календарь. Применяется только если календарь не является базовым."
type: docs
weight: 40
url: /ru/net/aspose.tasks/calendar/basecalendar/
---
## Calendar.BaseCalendar property

Получает или задает базовый календарь, от которого зависит этот календарь. Применяется только если календарь не является базовым.

```csharp
public Calendar BaseCalendar { get; set; }
```

## Примеры

Показывает, как работать с базовым календарем календаря ресурса.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var resource = project.Resources.Add("Resource1");

// Добавить стандартный календарь и назначить его ресурсу
var calendar = project.Calendars.Add("Resource1");
resource.Set(Rsc.Calendar, calendar);

// Отобразить название базового календаря для всех ресурсов
foreach (var rsc in project.Resources)
{
    if (rsc.Get(Rsc.Name) != null)
    {
        Console.WriteLine(rsc.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### См. также

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


