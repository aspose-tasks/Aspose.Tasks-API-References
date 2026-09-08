---
title: "WorkUnit.WorkUnit"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор WorkUnit. Инициализирует новый экземпляр класса WorkUnit. Создаёт новый объект WorkUnit с указанными датами From и To"
type: docs
weight: 10
url: /ru/net/aspose.tasks/workunit/workunit/
---
## WorkUnit constructor

Инициализирует новый экземпляр класса [`WorkUnit`](../). Создаёт новый объект WorkUnit с указанными датами From и To.

```csharp
public WorkUnit(DateTime from, DateTime to)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| от | DateTime | Дата начала рабочего времени. |
| по | DateTime | Дата окончания рабочего времени. |

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


