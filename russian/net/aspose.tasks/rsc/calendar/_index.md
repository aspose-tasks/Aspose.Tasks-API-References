---
title: "Rsc.Calendar"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Rsc field. Календарь ресурса"
type: docs
weight: 190
url: /ru/net/aspose.tasks/rsc/calendar/
---
## Rsc.Calendar field

Календарь ресурса.

```csharp
public static readonly Key<Calendar, RscKey> Calendar;
```

## Примеры

Показывает, как получить/установить календарь ресурса.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var res = project.Resources.Add("Resource1");

// Добавить стандартный календарь и назначить его ресурсу
var cal = project.Calendars.Add("Resource1");
res.Set(Rsc.Calendar, cal);

// Отобразить название базового календаря для всех ресурсов
foreach (var resource in project.Resources)
{
    if (resource.Get(Rsc.Name) != null)
    {
        Console.WriteLine(resource.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


