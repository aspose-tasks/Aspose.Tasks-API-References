---
title: "WorkUnit.From"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство WorkUnit. Возвращает или задает дату From"
type: docs
weight: 20
url: /ru/net/aspose.tasks/workunit/from/
---
## WorkUnit.From property

Получает или задаёт дату From.

```csharp
public DateTime From { get; set; }
```

## Примеры

Показывает, как работать с информацией о рабочей единице.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// получить рабочие часы для конкретной даты
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

Console.WriteLine("From: " + workUnit.From);
Console.WriteLine("To: " + workUnit.To);
Console.WriteLine("Working hours: " + workUnit.WorkingHours);
```

### См. также

* class [WorkUnit](../)
* namespace [Aspose.Tasks](../../workunit/)
* assembly [Aspose.Tasks](../../../)


