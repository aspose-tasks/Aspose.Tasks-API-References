---
title: "Tsk.PercentComplete"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Текущий статус задачи, выраженный в процентах от длительности задачи, которые завершены"
type: docs
weight: 880
url: /ru/net/aspose.tasks/tsk/percentcomplete/
---
## Tsk.PercentComplete field

Текущий статус задачи, выраженный в процентах от её длительности, который уже выполнен.

```csharp
public static readonly Key<int, TaskKey> PercentComplete;
```

## Примеры

Показывает, как изменить прогресс задачи, обновив процент завершения задачи.

```csharp
var project = new Project();
Console.WriteLine("Project Calculation mode is Automatic: {0}", project.CalculationMode.Equals(CalculationMode.Automatic));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(2));
task.Set(Tsk.PercentComplete, 50);

// Получите доступ к задачам и отобразите процент выполнения
foreach (var tsk in project.RootTask.Children)
{
    Console.WriteLine(tsk.Get(Tsk.PercentComplete));
    Console.WriteLine(tsk.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(tsk.Get(Tsk.PhysicalPercentComplete));
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


