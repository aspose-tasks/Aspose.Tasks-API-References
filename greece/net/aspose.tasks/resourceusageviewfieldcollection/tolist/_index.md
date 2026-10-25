---
title: "ResourceUsageViewFieldCollection.ToList"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ResourceUsageViewFieldCollection μέθοδος. Μετατρέπει το στιγμιότυπο της κλάσης ResourceUsageViewFieldCollection σε λίστα που περιέχει τα στιγμιότυπα της κλάσης ResourceUsageViewField"
type: docs
weight: 20
url: /el/net/aspose.tasks/resourceusageviewfieldcollection/tolist/
---
## ResourceUsageViewFieldCollection.ToList method

Μετατρέπει το στιγμιότυπο της κλάσης [`ResourceUsageViewFieldCollection`](../) σε λίστα που περιέχει τα στιγμιότυπα της κλάσης [`ResourceUsageViewField`](../../resourceusageviewfield/).

```csharp
public IList<ResourceUsageViewField> ToList()
```

### Τιμή Επιστροφής

Το στιγμιότυπο της κλάσης [`ResourceUsageViewFieldCollection`](../) μετατράπηκε σε λίστα που περιέχει τα στιγμιότυπα της κλάσης [`ResourceUsageViewField`](../../resourceusageviewfield/).

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τη συλλογή πεδίων ενός στιγμιότυπου ResourceUsageView.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// Μπορεί κανείς να μετατρέψει τη συλλογή σε λίστα του ResourceUsageViewField.
IList<ResourceUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### Δείτε επίσης

* enum [ResourceUsageViewField](../../resourceusageviewfield/)
* class [ResourceUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../resourceusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


