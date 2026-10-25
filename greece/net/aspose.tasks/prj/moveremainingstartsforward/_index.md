---
title: "Prj.MoveRemainingStartsForward"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν η έναρξη των εναπομείναντων τμημάτων των εργασιών που έχουν προγραμματιστεί να ξεκινήσουν αργότερα πρέπει να μετακινηθεί προς την ημερομηνία κατάστασης"
type: docs
weight: 520
url: /el/net/aspose.tasks/prj/moveremainingstartsforward/
---
## Prj.MoveRemainingStartsForward field

Καθορίζει εάν η έναρξη των εναπομείναντων τμημάτων των εργασιών που προγραμματίζονται να ξεκινήσουν αργότερα πρέπει να μεταφερθεί προς τα εμπρός στην ημερομηνία κατάστασης.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsForward;
```

## Παραδείγματα

Εμφανίζει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.MoveRemainingStartsForward.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsForward, true);

Console.WriteLine("Move Remaining Starts Forward: " + project.Get(Prj.MoveRemainingStartsForward));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


