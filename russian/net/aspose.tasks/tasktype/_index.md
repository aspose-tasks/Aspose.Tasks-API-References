---
title: "Перечисление TaskType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.TaskType перечисление. Указывает тип задачи"
type: docs
weight: 2470
url: /ru/net/aspose.tasks/tasktype/
---
## TaskType enumeration

Указывает тип задачи.

```csharp
public enum TaskType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `-1` | Неопределённое значение означает, что поле не было определено в оригинальном файле |
| FixedUnits | `0` | Фиксированные единицы |
| FixedDuration | `1` | Фиксированная продолжительность |
| FixedWork | `2` | Фиксированная работа |

## Примечания

При экспорте в XML неопределённые значения будут удалены из результирующего XML.

## Примеры

Показывает, как прочитать свойства проекта по умолчанию.

```csharp
var project = new Project(DataDir + "DefaultProperties.mpp");

// Установить свойства по умолчанию
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime, project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);

// Отобразить свойства по умолчанию
Console.WriteLine("New Task Default Start: " + project.Get(Prj.DefaultStartTime).ToShortDateString());
Console.WriteLine("New Task Default Type: " + project.Get(Prj.DefaultTaskType));
Console.WriteLine("Resource Default Standard Rate: " + project.Get(Prj.DefaultStandardRate));
Console.WriteLine("Resource Default Overtime Rate: " + project.Get(Prj.DefaultOvertimeRate));
Console.WriteLine("Default Task EV Method: " + project.Get(Prj.DefaultTaskEVMethod));
Console.WriteLine("Default Cost Accrual: " + project.Get(Prj.DefaultFixedCostAccrual));
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


