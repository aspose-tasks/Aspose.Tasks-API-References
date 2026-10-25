---
title: "Tsk.CV"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Разница между базовой стоимостью и общей стоимостью задачи. Отклонение стоимости  Стоимость  Базовая стоимость"
type: docs
weight: 260
url: /ru/net/aspose.tasks/tsk/cv/
---
## Tsk.CV field

Разница между базовой стоимостью и общей стоимостью задачи. Отклонение стоимости = Стоимость - Базовая стоимость.

```csharp
public static readonly Key<double, TaskKey> CV;
```

## Примеры

Показывает, как читать значения стоимости задачи.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (var task in collector.Tasks)
{
    Console.WriteLine("Cost: " + task.Get(Tsk.Cost));
    Console.WriteLine("ACWP: " + task.Get(Tsk.ACWP));
    Console.WriteLine("BCWP: " + task.Get(Tsk.BCWP));
    Console.WriteLine("BCWS: " + task.Get(Tsk.BCWS));

    // CV = BCWP - ACWP
    Console.WriteLine("CV: " + task.Get(Tsk.CV));
    Console.WriteLine();
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


