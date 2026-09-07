---
title: "SplitPartCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "SplitPartCollection μέθοδος. Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή"
type: docs
weight: 30
url: /el/net/aspose.tasks/splitpartcollection/getenumerator/
---
## SplitPartCollection.GetEnumerator method

Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή.

```csharp
public IEnumerator<SplitPart> GetEnumerator()
```

### Τιμή Επιστροφής

έναν απαριθμητή για αυτή τη συλλογή.

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

* class [SplitPart](../../splitpart/)
* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


