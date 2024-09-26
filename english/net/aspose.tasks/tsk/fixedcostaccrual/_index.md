---
title: Tsk.FixedCostAccrual
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines choices for how and when fixed costs are to be charged or accrued to the cost of a task
type: docs
weight: 440
url: /net/aspose.tasks/tsk/fixedcostaccrual/
---
## Tsk.FixedCostAccrual field

Determines choices for how and when fixed costs are to be charged, or accrued, to the cost of a task.

```csharp
public static readonly Key<CostAccrualType, TaskKey> FixedCostAccrual;
```

## Examples

Shows how to read/write Tsk.FixedCostAccrual property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FixedCostAccrual, CostAccrualType.Prorated);

Console.WriteLine("Fixed Cost Accrual: " + task.Get(Tsk.FixedCostAccrual));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


