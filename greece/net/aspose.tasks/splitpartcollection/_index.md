---
title: "Κλάση SplitPartCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.SplitPartCollection class. Συλλογή που αντιπροσωπεύει τα τμήματα μιας εργασίας."
type: docs
weight: 2300
url: /el/net/aspose.tasks/splitpartcollection/
---
## SplitPartCollection class

Συλλογή που αντιπροσωπεύει τα τμήματα μιας εργασίας.

```csharp
public class SplitPartCollection : IList<SplitPart>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/splitpartcollection/count/) { get; } | Λαμβάνει τον αριθμό των τμημάτων στη συλλογή. |
| [Item](../../aspose.tasks/splitpartcollection/item/) { get; set; } | Ανακτά το τμήμα διαίρεσης μιας εργασίας στο συγκεκριμένο δείκτη. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/splitpartcollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [ToArray](../../aspose.tasks/splitpartcollection/toarray/)() | Αντιγράφει όλα τα τμήματα από τη συλλογή σε έναν νέο πίνακα. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές τμημάτων διαίρεσης.

```csharp
var project = new Project(DataDir + "Splits.mpp");

var task = project.RootTask.Children.GetById(1);

// επανάληψη πάνω από τα τμήματα διαίρεσης
Console.WriteLine("Iterate over split parts");
Console.WriteLine("Split parts count:" + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("Start: " + splitPart.Start);
    Console.WriteLine("Finish: " + splitPart.Finish);
}

// λάβετε το τμήμα με βάση το δείκτη
var split = task.SplitParts[0];
Console.WriteLine("Split start: " + split.Start);

// κάντε κάποια εργασία με το πρώτο τμήμα διαίρεσης της εργασίας
```

### Δείτε επίσης

* class [SplitPart](../splitpart/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


