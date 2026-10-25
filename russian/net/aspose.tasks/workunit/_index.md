---
title: "Класс WorkUnit"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.WorkUnit. Представляет рабочие часы"
type: docs
weight: 3630
url: /ru/net/aspose.tasks/workunit/
---
## WorkUnit class

Представляет рабочие часы.

```csharp
public class WorkUnit
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WorkUnit](workunit/)(DateTime, DateTime) | Инициализирует новый экземпляр класса `WorkUnit`. Создаёт новый объект WorkUnit с указанными датами From и To. |

## Свойства

| Имя | Описание |
| --- | --- |
| [From](../../aspose.tasks/workunit/from/) { get; set; } | Получает или задаёт дату From. |
| [To](../../aspose.tasks/workunit/to/) { get; set; } | Получает или задаёт дату To. |
| [WorkingHours](../../aspose.tasks/workunit/workinghours/) { get; set; } | Получает или задаёт продолжительность рабочих часов. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


