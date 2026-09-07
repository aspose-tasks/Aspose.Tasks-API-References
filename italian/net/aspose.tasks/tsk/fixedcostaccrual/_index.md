---
title: "Tsk.FixedCostAccrual"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina le scelte su come e quando i costi fissi devono essere addebitati o accreditati al costo di un'attività"
type: docs
weight: 440
url: /it/net/aspose.tasks/tsk/fixedcostaccrual/
---
## Tsk.FixedCostAccrual field

Determina le opzioni su come e quando i costi fissi devono essere addebitati o accreditati al costo di un'attività.

```csharp
public static readonly Key<CostAccrualType, TaskKey> FixedCostAccrual;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.FixedCostAccrual.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FixedCostAccrual, CostAccrualType.Prorated);

Console.WriteLine("Fixed Cost Accrual: " + task.Get(Tsk.FixedCostAccrual));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


