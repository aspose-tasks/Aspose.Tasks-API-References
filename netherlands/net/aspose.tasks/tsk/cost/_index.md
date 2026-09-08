---
title: "Tsk.Cost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De totale geplande of geprojecteerde kosten voor een taak op basis van reeds gemaakte kosten voor werk uitgevoerd door aan de taak toegewezen resources, naast de kosten die gepland zijn voor het resterende werk"
type: docs
weight: 230
url: /nl/net/aspose.tasks/tsk/cost/
---
## Tsk.Cost field

De totale geplande of verwachte kosten voor een taak op basis van reeds gemaakte kosten voor werk uitgevoerd door aan de taak toegewezen resources, naast de kosten die gepland zijn voor het resterende werk.

```csharp
public static readonly Key<decimal, TaskKey> Cost;
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


