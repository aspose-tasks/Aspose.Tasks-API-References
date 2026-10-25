---
title: "Tsk.OvertimeCost"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Общая стоимость сверхурочных для задачи по ресурсу на всех назначенных задачах или для назначения ресурса"
type: docs
weight: 860
url: /ru/net/aspose.tasks/tsk/overtimecost/
---
## Tsk.OvertimeCost field

Общая стоимость сверхурочной работы для задачи, ресурса по всем назначенным задачам или для назначения ресурса.

```csharp
public static readonly Key<decimal, TaskKey> OvertimeCost;
```

## Примеры

Показывает, как читать сверхурочные задачи.

```csharp
var project = new Project(DataDir + "TaskOvertimes.mpp");

// Читать сверхурочные и процент завершения задач
foreach (var task in project.RootTask.Children)
{
    Console.WriteLine(task.Get(Tsk.OvertimeCost));
    Console.WriteLine(task.Get(Tsk.OvertimeWork));
    Console.WriteLine(task.Get(Tsk.PercentComplete));
    Console.WriteLine(task.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(task.Get(Tsk.PhysicalPercentComplete));

    // Установить процент завершения
    task.Set(Tsk.PercentComplete, 100);
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


