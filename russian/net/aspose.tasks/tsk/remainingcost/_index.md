---
title: "Tsk.RemainingCost"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Tsk field. Оставшиеся запланированные расходы, которые будут понесены при выполнении оставшейся запланированной работы"
type: docs
weight: 950
url: /ru/net/aspose.tasks/tsk/remainingcost/
---
## Tsk.RemainingCost field

Оставшиеся запланированные расходы, которые будут понесены при выполнении оставшейся запланированной работы.

```csharp
public static readonly Key<decimal, TaskKey> RemainingCost;
```

## Примеры

Показывает, как читать затраты задачи.

```csharp
var project = new Project();

// Добавить задачу и установить стоимость
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Cost, 800);

// Отобразить свойства задачи, связанные со стоимостью
Console.WriteLine(task.Get(Tsk.RemainingCost));
Console.WriteLine(task.Get(Tsk.FixedCost));
Console.WriteLine(task.Get(Tsk.CostVariance));
Console.WriteLine(project.RootTask.Get(Tsk.Cost));
Console.WriteLine(project.RootTask.Get(Tsk.FixedCost));
Console.WriteLine(project.RootTask.Get(Tsk.RemainingCost));
Console.WriteLine(project.RootTask.Get(Tsk.CostVariance));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


