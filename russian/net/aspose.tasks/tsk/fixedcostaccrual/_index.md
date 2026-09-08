---
title: "Tsk.FixedCostAccrual"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет варианты того, как и когда фиксированные затраты должны быть начислены или отнесены к стоимости задачи"
type: docs
weight: 440
url: /ru/net/aspose.tasks/tsk/fixedcostaccrual/
---
## Tsk.FixedCostAccrual field

Определяет варианты того, как и когда фиксированные расходы должны быть начислены или отложены к стоимости задачи.

```csharp
public static readonly Key<CostAccrualType, TaskKey> FixedCostAccrual;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.FixedCostAccrual.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FixedCostAccrual, CostAccrualType.Prorated);

Console.WriteLine("Fixed Cost Accrual: " + task.Get(Tsk.FixedCostAccrual));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


