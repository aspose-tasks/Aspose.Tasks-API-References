---
title: "FieldHelper.GetDefaultTaskFieldTitle"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος FieldHelper. Επιστρέφει έναν προεπιλεγμένο τίτλο του συγκεκριμένου πεδίου εργασίας"
type: docs
weight: 20
url: /el/net/aspose.tasks.util/fieldhelper/getdefaulttaskfieldtitle/
---
## FieldHelper.GetDefaultTaskFieldTitle method

Επιστρέφει έναν προεπιλεγμένο τίτλο του συγκεκριμένου πεδίου εργασίας.

```csharp
public static string GetDefaultTaskFieldTitle(TaskKey taskKey)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| taskKey | TaskKey | Πεδίο εργασίας για λήψη προεπιλεγμένου τίτλου. |

### Τιμή Επιστροφής

Ένας προεπιλεγμένος τίτλος του συγκεκριμένου πεδίου εργασίας εάν το πεδίο μπορεί να εμφανιστεί στην προβολή του MS Project, αλλιώς null.

## Παραδείγματα

Δείχνει πώς να λάβετε τον προεπιλεγμένο τίτλο πεδίου για το συγκεκριμένο πεδίο εργασίας.

```csharp
Console.WriteLine("Title for Tsk.ActualCost: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.ActualCost.KeyType));
Console.WriteLine("Title for Tsk.PercentWorkComplete: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.PercentWorkComplete.KeyType));
```

### Δείτε επίσης

* enum [TaskKey](../../../aspose.tasks/taskkey/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


