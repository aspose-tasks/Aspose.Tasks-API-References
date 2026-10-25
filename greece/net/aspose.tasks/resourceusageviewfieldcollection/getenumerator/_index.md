---
title: "ResourceUsageViewFieldCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ResourceUsageViewFieldCollection μέθοδος. Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή"
type: docs
weight: 10
url: /el/net/aspose.tasks/resourceusageviewfieldcollection/getenumerator/
---
## ResourceUsageViewFieldCollection.GetEnumerator method

Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή.

```csharp
public IEnumerator<ResourceUsageViewField> GetEnumerator()
```

### Τιμή Επιστροφής

έναν απαριθμητή για αυτή τη συλλογή.

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


