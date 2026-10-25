---
title: "BaselineCollection.ParentResource"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα BaselineCollection. Λαμβάνει το γονικό Resource για αυτή τη συλλογή"
type: docs
weight: 30
url: /el/net/aspose.tasks/baselinecollection/parentresource/
---
## BaselineCollection.ParentResource property

Λαμβάνει το γονικό [`Resource`](../../resource/) για αυτή τη συλλογή.

```csharp
public Resource ParentResource { get; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές baseline.

```csharp
var project = new Project(DataDir + "WorkWithBaselineCollection.mpp");
var resource = project.Resources.GetByUid(1);

Console.WriteLine("Count of assignment baselines: " + resource.Baselines.Count);
Console.WriteLine("Parent Resource Name: " + resource.Baselines.ParentResource.Get(Rsc.Name));

// διαβάστε πληροφορίες baseline
foreach (var baseline in resource.Baselines)
{
    Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
    Console.WriteLine("Cost: " + baseline.Cost);
    Console.WriteLine("Work: " + baseline.Work);
    Console.WriteLine("BCWP: " + baseline.Bcwp);
    Console.WriteLine("BCWS: " + baseline.Bcws);
    Console.WriteLine();
}

Console.WriteLine("Delete all baselines: ");
List<Baseline> baselines = resource.Baselines.ToList();
foreach (var baseline in baselines)
{
    Console.WriteLine("Delete baseline with name: " + baseline.BaselineNumber);
    resource.Baselines.Remove(baseline);
}
```

### Δείτε επίσης

* class [Resource](../../resource/)
* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


