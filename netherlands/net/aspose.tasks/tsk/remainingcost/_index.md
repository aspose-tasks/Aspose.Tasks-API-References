---
title: "Tsk.RemainingCost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De resterende geplande uitgave die zal worden gemaakt bij het voltooien van het resterende geplande werk"
type: docs
weight: 950
url: /nl/net/aspose.tasks/tsk/remainingcost/
---
## Tsk.RemainingCost field

De resterende geplande kosten die gemaakt zullen worden bij het voltooien van het resterende geplande werk.

```csharp
public static readonly Key<decimal, TaskKey> RemainingCost;
```

## Voorbeelden

Toont hoe taakkosten te lezen.

```csharp
var project = new Project();

// Voeg taak toe en stel kosten in
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Cost, 800);

// Toon kostengerelateerde eigenschappen van taak
Console.WriteLine(task.Get(Tsk.RemainingCost));
Console.WriteLine(task.Get(Tsk.FixedCost));
Console.WriteLine(task.Get(Tsk.CostVariance));
Console.WriteLine(project.RootTask.Get(Tsk.Cost));
Console.WriteLine(project.RootTask.Get(Tsk.FixedCost));
Console.WriteLine(project.RootTask.Get(Tsk.RemainingCost));
Console.WriteLine(project.RootTask.Get(Tsk.CostVariance));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


