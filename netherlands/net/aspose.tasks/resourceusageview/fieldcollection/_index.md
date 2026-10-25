---
title: "ResourceUsageView.FieldCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceUsageView‑eigenschap. Haalt het ResourceUsageViewFieldCollection‑object op van deze ResourceUsageView"
type: docs
weight: 10
url: /nl/net/aspose.tasks/resourceusageview/fieldcollection/
---
## ResourceUsageView.FieldCollection property

Haalt het [`ResourceUsageViewFieldCollection`](../../resourceusageviewfieldcollection/)‑object op van deze ResourceUsageView.

```csharp
public ResourceUsageViewFieldCollection FieldCollection { get; }
```

## Voorbeelden

Toont hoe resourcegebruik‑weergavevelden gelezen moeten worden.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### Zie ook

* class [ResourceUsageViewFieldCollection](../../resourceusageviewfieldcollection/)
* class [ResourceUsageView](../)
* namespace [Aspose.Tasks](../../resourceusageview/)
* assembly [Aspose.Tasks](../../../)


