---
title: "Class VbaModuleAttribute"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.VbaModuleAttribute class. Το χαρακτηριστικό του αντικειμένου VbaModule"
type: docs
weight: 2820
url: /el/net/aspose.tasks/vbamoduleattribute/
---
## VbaModuleAttribute class

Το χαρακτηριστικό του αντικειμένου [`VbaModule`](../vbamodule/)

```csharp
public sealed class VbaModuleAttribute : IEquatable<VbaModuleAttribute>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Key](../../aspose.tasks/vbamoduleattribute/key/) { get; } | Αποκτά το κλειδί του χαρακτηριστικού μονάδας VBA. |
| [Value](../../aspose.tasks/vbamoduleattribute/value/) { get; } | Αποκτά την τιμή του χαρακτηριστικού μονάδας VBA. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals_1)(object) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο `VbaModuleAttribute`. |
| [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals)(VbaModuleAttribute) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο `VbaModuleAttribute`. |
| override [GetHashCode](../../aspose.tasks/vbamoduleattribute/gethashcode/)() | Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το `VbaModuleAttribute`. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τις ιδιότητες της μονάδας VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("  VB Name: " + attribute.Key);
        Console.WriteLine("  Module: " + attribute.Value);
    }
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


