---
title: "TaskUsageViewFieldCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος TaskUsageViewFieldCollection. Επιστρέφει έναν επαναλήπτη για αυτή τη συλλογή"
type: docs
weight: 10
url: /el/net/aspose.tasks/taskusageviewfieldcollection/getenumerator/
---
## TaskUsageViewFieldCollection.GetEnumerator method

Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή.

```csharp
public IEnumerator<TaskUsageViewField> GetEnumerator()
```

### Τιμή Επιστροφής

έναν απαριθμητή για αυτή τη συλλογή.

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τη συλλογή πεδίων μιας παρουσίας TaskUsageView.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// Μπορεί κανείς να μετατρέψει τη συλλογή σε λίστα των TaskUsageViewField.
IList<TaskUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### Δείτε επίσης

* enum [TaskUsageViewField](../../taskusageviewfield/)
* class [TaskUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../taskusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


