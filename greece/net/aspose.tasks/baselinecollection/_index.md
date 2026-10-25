---
title: "Κλάση BaselineCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.BaselineCollection. Αντιπροσωπεύει μια συλλογή αντικειμένων Baseline"
type: docs
weight: 120
url: /el/net/aspose.tasks/baselinecollection/
---
## BaselineCollection class

Αντιπροσωπεύει μια συλλογή αντικειμένων [`Baseline`](../baseline/).

```csharp
public class BaselineCollection : IList<Baseline>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/baselinecollection/count/) { get; } | Επιστρέφει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο BaselineCollection. |
| [Item](../../aspose.tasks/baselinecollection/item/) { get; set; } | Επιστρέφει το στοιχείο στο καθορισμένο δείκτη. |
| [ParentResource](../../aspose.tasks/baselinecollection/parentresource/) { get; } | Επιστρέφει το γονικό [`Resource`](../resource/) για αυτή τη συλλογή. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/baselinecollection/add/)(Baseline) | Αυτή είναι η ψευδοεφαρμογή της μεθόδου Add του ICollection, η οποία μόνο ρίχνει NotSupportedException |
| [GetEnumerator](../../aspose.tasks/baselinecollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [Remove](../../aspose.tasks/baselinecollection/remove/)(Baseline) | Αφαιρεί το baseline από αυτή τη συλλογή. |
| [ToList](../../aspose.tasks/baselinecollection/tolist/)() | Μετατρέπει το αντικείμενο BaselineCollection σε λίστα αντικειμένων [`Baseline`](../baseline/). |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


