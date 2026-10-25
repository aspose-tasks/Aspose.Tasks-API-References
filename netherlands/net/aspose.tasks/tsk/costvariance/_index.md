---
title: "Tsk.CostVariance"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Het verschil tussen de basiskost en de totale kost voor een taakresource of -toewijzing."
type: docs
weight: 240
url: /nl/net/aspose.tasks/tsk/costvariance/
---
## Tsk.CostVariance field

Het verschil tussen de basislijnkosten en de totale kosten voor een taak, resource of toewijzing.

```csharp
public static readonly Key<double, TaskKey> CostVariance;
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


