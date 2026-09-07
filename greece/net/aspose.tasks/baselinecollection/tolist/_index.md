---
title: "BaselineCollection.ToList"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "BaselineCollection μέθοδος. Μετατρέπει το αντικείμενο BaselineCollection σε λίστα αντικειμένων Baseline"
type: docs
weight: 70
url: /el/net/aspose.tasks/baselinecollection/tolist/
---
## BaselineCollection.ToList method

Μετατρέπει το αντικείμενο BaselineCollection σε λίστα αντικειμένων [`Baseline`](../../baseline/).

```csharp
public List<Baseline> ToList()
```

### Τιμή Επιστροφής

Λίστα αντικειμένων [`Baseline`](../../baseline/).

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


