---
title: "TaskUsageView.FieldCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα TaskUsageView. Λαμβάνει το αντικείμενο TaskUsageViewFieldCollection αυτού του TaskUsageView"
type: docs
weight: 10
url: /el/net/aspose.tasks/taskusageview/fieldcollection/
---
## TaskUsageView.FieldCollection property

Λαμβάνει το αντικείμενο [`TaskUsageViewFieldCollection`](../../taskusageviewfieldcollection/) αυτού του TaskUsageView.

```csharp
public TaskUsageViewFieldCollection FieldCollection { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τα πεδία προβολής χρήσης εργασίας.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### Δείτε επίσης

* class [TaskUsageViewFieldCollection](../../taskusageviewfieldcollection/)
* class [TaskUsageView](../)
* namespace [Aspose.Tasks](../../taskusageview/)
* assembly [Aspose.Tasks](../../../)


