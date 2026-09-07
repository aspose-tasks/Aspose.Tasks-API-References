---
title: "ResourceUsageView.FieldCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ResourceUsageView. Λαμβάνει το αντικείμενο ResourceUsageViewFieldCollection αυτής της ResourceUsageView."
type: docs
weight: 10
url: /el/net/aspose.tasks/resourceusageview/fieldcollection/
---
## ResourceUsageView.FieldCollection property

Λαμβάνει το αντικείμενο [`ResourceUsageViewFieldCollection`](../../resourceusageviewfieldcollection/) αυτής της ResourceUsageView.

```csharp
public ResourceUsageViewFieldCollection FieldCollection { get; }
```

## Παραδείγματα

Εμφανίζει πώς να διαβάσετε τα πεδία προβολής χρήσης πόρων.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### Δείτε επίσης

* class [ResourceUsageViewFieldCollection](../../resourceusageviewfieldcollection/)
* class [ResourceUsageView](../)
* namespace [Aspose.Tasks](../../resourceusageview/)
* assembly [Aspose.Tasks](../../../)


