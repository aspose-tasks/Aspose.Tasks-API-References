---
title: "Prj.AutoCalculateAssignmentCosts"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se il costo dell'assegnazione e il costo residuo devono essere calcolati automaticamente usando il lavoro delle assegnazioni e le tariffe delle risorse"
type: docs
weight: 60
url: /it/net/aspose.tasks/prj/autocalculateassignmentcosts/
---
## Prj.AutoCalculateAssignmentCosts field

Determina se il costo dell'assegnazione e il costo residuo devono essere calcolati automaticamente utilizzando il lavoro dell'assegnazione e le tariffe delle risorse.

```csharp
public static readonly Key<bool, PrjKey> AutoCalculateAssignmentCosts;
```

## Esempi

Mostra come disattivare il calcolo automatico dei costi dell'assegnazione e impostare i costi dell'assegnazione esplicitamente.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("New task");
task.Duration = project.GetDuration(TimeSpan.FromHours(15), TimeUnitType.Day);
var resource = project.Resources.Add("Resource");
resource.StandardRate = 10m;

var assignment = project.ResourceAssignments.Add(task, resource);

assignment.Work = project.GetDuration(TimeSpan.FromHours(12), TimeUnitType.Day);
assignment.ActualWork = project.GetDuration(TimeSpan.FromHours(3), TimeUnitType.Day);

Console.WriteLine("Now assignment's cost are auto calculated:");
Console.WriteLine("Actual Cost: {0}", assignment.ActualCost);
Console.WriteLine("Remaining Cost: {0}", assignment.RemainingCost);
Console.WriteLine("Cost: {0}", assignment.Cost);

project.AutoCalculateAssignmentCosts = false;
assignment.ActualCost = 123;
assignment.RemainingCost = 456;
assignment.Cost = 555;

Console.WriteLine("Now auto calculation of assignment's cost is turned off.");
Console.WriteLine("Actual Cost: {0}", assignment.ActualCost);
Console.WriteLine("Remaining Cost: {0}", assignment.RemainingCost);
Console.WriteLine("Cost: {0}", assignment.Cost);
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


