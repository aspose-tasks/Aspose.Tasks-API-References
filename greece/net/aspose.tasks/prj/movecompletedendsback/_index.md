---
title: "Prj.MoveCompletedEndsBack"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν το τέλος των ολοκληρωμένων τμημάτων εργασιών που προγραμματίστηκαν να ξεκινήσουν μετά την ημερομηνία κατάστασης αλλά ξεκίνησαν νωρίτερα πρέπει να μεταφερθεί πίσω στην ημερομηνία κατάστασης"
type: docs
weight: 490
url: /el/net/aspose.tasks/prj/movecompletedendsback/
---
## Prj.MoveCompletedEndsBack field

Καθορίζει εάν το τέλος των ολοκληρωμένων τμημάτων των εργασιών που προγραμματίζονται να ξεκινήσουν μετά την ημερομηνία κατάστασης αλλά ξεκίνησαν νωρίτερα πρέπει να μετακινηθεί πίσω στην ημερομηνία κατάστασης.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsBack;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.MoveCompletedEndsBack.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsBack, true);

Console.WriteLine("Move Completed Ends Back: " + project.Get(Prj.MoveCompletedEndsBack));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


