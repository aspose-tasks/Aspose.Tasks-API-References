---
title: "Prj.MoveRemainingStartsBack"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν η αρχή των εναπομείναντων τμημάτων των εργασιών που προγραμματίζονται να ξεκινήσουν μετά την ημερομηνία κατάστασης αλλά ξεκίνησαν νωρίτερα πρέπει να μεταφερθεί πίσω στην ημερομηνία κατάστασης."
type: docs
weight: 510
url: /el/net/aspose.tasks/prj/moveremainingstartsback/
---
## Prj.MoveRemainingStartsBack field

Καθορίζει εάν η έναρξη των εναπομείναντων τμημάτων των εργασιών που προγραμματίζονται να ξεκινήσουν μετά την ημερομηνία κατάστασης αλλά ξεκίνησαν νωρίτερα πρέπει να μετακινηθεί πίσω στην ημερομηνία κατάστασης.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsBack;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.MoveRemainingStartsBack.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsBack, true);

Console.WriteLine("Move Remaining Starts Back: " + project.Get(Prj.MoveRemainingStartsBack));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


