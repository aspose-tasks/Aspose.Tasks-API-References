---
title: "Tsk.FixedCostAccrual"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Bepaalt de keuzes voor hoe en wanneer vaste kosten in rekening worden gebracht of worden toegerekend aan de kosten van een taak"
type: docs
weight: 440
url: /nl/net/aspose.tasks/tsk/fixedcostaccrual/
---
## Tsk.FixedCostAccrual field

Bepaalt keuzes voor hoe en wanneer vaste kosten in rekening worden gebracht of worden toegerekend aan de kosten van een taak.

```csharp
public static readonly Key<CostAccrualType, TaskKey> FixedCostAccrual;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.FixedCostAccrual te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FixedCostAccrual, CostAccrualType.Prorated);

Console.WriteLine("Fixed Cost Accrual: " + task.Get(Tsk.FixedCostAccrual));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


