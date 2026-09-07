---
title: "Prj.MoveCompletedEndsForward"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν το τέλος των ολοκληρωμένων τμημάτων των εργασιών που προγραμματίστηκαν να ολοκληρωθούν πριν από την ημερομηνία κατάστασης αλλά ξεκίνησαν αργότερα πρέπει να μεταφερθεί στην ημερομηνία κατάστασης"
type: docs
weight: 500
url: /el/net/aspose.tasks/prj/movecompletedendsforward/
---
## Prj.MoveCompletedEndsForward field

Καθορίζει εάν το τέλος των ολοκληρωμένων τμημάτων των εργασιών που προγραμματίζονται να έχουν ολοκληρωθεί πριν την ημερομηνία κατάστασης αλλά ξεκίνησαν αργότερα πρέπει να μετακινηθεί προς τα πάνω στην ημερομηνία κατάστασης.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsForward;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.MoveCompletedEndsForward.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsForward, true);

Console.WriteLine("Move Completed Ends Forward: " + project.Get(Prj.MoveCompletedEndsForward));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


