---
title: "Tsk.Cost"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Общая запланированная или прогнозируемая стоимость задачи, основанная на уже понесённых затратах за работу, выполненную ресурсами, назначенными на задачи, а также на затратах, запланированных для оставшейся работы"
type: docs
weight: 230
url: /ru/net/aspose.tasks/tsk/cost/
---
## Tsk.Cost field

Общая запланированная или прогнозируемая стоимость задачи, основанная на уже понесённых расходах за работу, выполненную ресурсами, назначенными на задачи, а также на расходах, запланированных для оставшейся работы.

```csharp
public static readonly Key<decimal, TaskKey> Cost;
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


