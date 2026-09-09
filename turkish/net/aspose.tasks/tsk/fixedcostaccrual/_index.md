---
title: "Tsk.FixedCostAccrual"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Sabit maliyetlerin bir görevin maliyetine ne zaman ve nasıl tahsil edileceği veya tahakkuk ettirileceği seçeneklerini belirler."
type: docs
weight: 440
url: /tr/net/aspose.tasks/tsk/fixedcostaccrual/
---
## Tsk.FixedCostAccrual field

Sabit maliyetlerin bir görevin maliyetine ne zaman ve nasıl yansıtılacağı veya tahakkuk ettirileceği seçeneklerini belirler.

```csharp
public static readonly Key<CostAccrualType, TaskKey> FixedCostAccrual;
```

## Örnekler

Tsk.FixedCostAccrual özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FixedCostAccrual, CostAccrualType.Prorated);

Console.WriteLine("Fixed Cost Accrual: " + task.Get(Tsk.FixedCostAccrual));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


