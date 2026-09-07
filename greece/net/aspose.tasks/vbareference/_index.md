---
title: "Κλάση VbaReference"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η κλάση Aspose.Tasks.VbaReference. Αντιπροσωπεύει μια αναφορά του VbaProject"
type: docs
weight: 2870
url: /el/net/aspose.tasks/vbareference/
---
## VbaReference class

Αναπαριστά μια αναφορά του [`VbaProject`](../vbaproject/).

```csharp
public sealed class VbaReference : IEquatable<VbaReference>
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [VbaReference](vbareference/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [LibIdentifier](../../aspose.tasks/vbareference/libidentifier/) { get; } | Λαμβάνει το αναγνωριστικό της βιβλιοθήκης. |
| [Name](../../aspose.tasks/vbareference/name/) { get; set; } | Λαμβάνει ή ορίζει το όνομα της αναφοράς VBA. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [Equals](../../aspose.tasks/vbareference/equals/#equals_1)(object) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο `VbaReference`. |
| [Equals](../../aspose.tasks/vbareference/equals/#equals)(VbaReference) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο `VbaReference`. |
| override [GetHashCode](../../aspose.tasks/vbareference/gethashcode/)() | Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το `VbaReference`. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε αναφορές VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


