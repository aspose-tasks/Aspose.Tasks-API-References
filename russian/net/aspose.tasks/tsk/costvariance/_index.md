---
title: "Tsk.CostVariance"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Разница между базовой стоимостью и общей стоимостью ресурса задачи или назначения"
type: docs
weight: 240
url: /ru/net/aspose.tasks/tsk/costvariance/
---
## Tsk.CostVariance field

Разница между базовой стоимостью и общей стоимостью задачи, ресурса или назначения.

```csharp
public static readonly Key<double, TaskKey> CostVariance;
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


