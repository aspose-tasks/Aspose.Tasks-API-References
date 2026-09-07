---
title: "Κλάση TaskUsageViewFieldCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.TaskUsageViewFieldCollection. Αντιπροσωπεύει μια συλλογή τιμών TaskUsageViewField."
type: docs
weight: 2500
url: /el/net/aspose.tasks/taskusageviewfieldcollection/
---
## TaskUsageViewFieldCollection class

Αντιπροσωπεύει μια συλλογή τιμών [`TaskUsageViewField`](../taskusageviewfield/).

```csharp
public class TaskUsageViewFieldCollection : IList<TaskUsageViewField>
```

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/taskusageviewfieldcollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [ToList](../../aspose.tasks/taskusageviewfieldcollection/tolist/)() | Επιστρέφει μια λίστα που περιέχει όλα τα στοιχεία από αυτή τη συλλογή. |

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

* enum [TaskUsageViewField](../taskusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


