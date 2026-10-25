---
title: "SplitPartCollection.ToArray"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "SplitPartCollection μέθοδος. Αντιγράφει όλα τα μέρη από τη συλλογή σε νέο πίνακα"
type: docs
weight: 40
url: /el/net/aspose.tasks/splitpartcollection/toarray/
---
## SplitPartCollection.ToArray method

Αντιγράφει όλα τα τμήματα από τη συλλογή σε έναν νέο πίνακα.

```csharp
public SplitPart[] ToArray()
```

### Τιμή Επιστροφής

Ένας πίνακας αντικειμένων [`SplitPart`](../../splitpart/).

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


