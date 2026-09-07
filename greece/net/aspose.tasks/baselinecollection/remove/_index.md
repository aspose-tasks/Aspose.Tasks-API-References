---
title: "BaselineCollection.Remove"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "BaselineCollection μέθοδος. Αφαιρεί το baseline από αυτή τη συλλογή"
type: docs
weight: 60
url: /el/net/aspose.tasks/baselinecollection/remove/
---
## BaselineCollection.Remove method

Αφαιρεί το baseline από αυτή τη συλλογή.

```csharp
public bool Remove(Baseline item)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | Baseline | Το στοιχείο προς αφαίρεση. |

### Τιμή Επιστροφής

true εάν η παρουσία [`Baseline`](../../baseline/) έχει αφαιρεθεί επιτυχώς· διαφορετικά false

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

* class [Baseline](../../baseline/)
* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


