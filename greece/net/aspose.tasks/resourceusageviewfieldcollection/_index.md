---
title: "Κλάση ResourceUsageViewFieldCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.ResourceUsageViewFieldCollection κλάση. Αντιπροσωπεύει μια συλλογή τιμών ResourceUsageViewField."
type: docs
weight: 1830
url: /el/net/aspose.tasks/resourceusageviewfieldcollection/
---
## ResourceUsageViewFieldCollection class

Αντιπροσωπεύει μια συλλογή τιμών [`ResourceUsageViewField`](../resourceusageviewfield/).

```csharp
public class ResourceUsageViewFieldCollection : IList<ResourceUsageViewField>
```

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/resourceusageviewfieldcollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [ToList](../../aspose.tasks/resourceusageviewfieldcollection/tolist/)() | Μετατρέπει το στιγμιότυπο της κλάσης `ResourceUsageViewFieldCollection` σε λίστα που περιέχει τα στιγμιότυπα της κλάσης [`ResourceUsageViewField`](../resourceusageviewfield/). |

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

* enum [ResourceUsageViewField](../resourceusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


