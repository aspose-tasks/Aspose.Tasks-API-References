---
title: "TaskUsageViewFieldCollection.ToList"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος TaskUsageViewFieldCollection. Επιστρέφει μια λίστα που περιέχει όλα τα στοιχεία από αυτή τη συλλογή"
type: docs
weight: 20
url: /el/net/aspose.tasks/taskusageviewfieldcollection/tolist/
---
## TaskUsageViewFieldCollection.ToList method

Επιστρέφει μια λίστα που περιέχει όλα τα στοιχεία από αυτή τη συλλογή.

```csharp
public IList<TaskUsageViewField> ToList()
```

### Τιμή Επιστροφής

επιστρέφει μια λίστα που περιέχει όλα τα στοιχεία από αυτή τη συλλογή.

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


