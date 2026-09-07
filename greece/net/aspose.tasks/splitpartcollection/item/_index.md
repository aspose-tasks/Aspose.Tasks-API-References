---
title: "SplitPartCollection.Item"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "SplitPartCollection ιδιότητα. Ανακτά ένα τμήμα διαχωρισμού εργασιών στον δεδομένο δείκτη"
type: docs
weight: 20
url: /el/net/aspose.tasks/splitpartcollection/item/
---
## SplitPartCollection indexer

Ανακτά το τμήμα διαίρεσης μιας εργασίας στο συγκεκριμένο δείκτη.

```csharp
public SplitPart this[int index] { get; set; }
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| index | Ο δείκτης του τμήματος. |

### Τιμή Επιστροφής

ένα τμήμα διαχωρισμού.

## Παρατηρήσεις

Ο δείκτης είναι μηδενικής βάσης. Επιστρέφει null εάν ο δείκτης βρίσκεται εκτός των ορίων του πίνακα.

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


