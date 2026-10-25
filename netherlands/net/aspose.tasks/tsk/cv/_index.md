---
title: "Tsk.CV"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk field. Het verschil tussen de baseline cost en de total cost voor een taak. Cost Variance  Cost  Baseline Cost"
type: docs
weight: 260
url: /nl/net/aspose.tasks/tsk/cv/
---
## Tsk.CV field

Het verschil tussen de basislijnkosten en de totale kosten voor een taak. Kostenvariatie = Kosten - Basislijnkosten

```csharp
public static readonly Key<double, TaskKey> CV;
```

## Voorbeelden

Toont hoe taakkostwaarden gelezen kunnen worden.

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

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


