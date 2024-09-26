---
title: ResourceUsageView.FieldCollection
second_title: Aspose.Tasks for .NET API Reference
description: ResourceUsageView property. Gets the ResourceUsageViewFieldCollection object of this ResourceUsageView
type: docs
weight: 10
url: /net/aspose.tasks/resourceusageview/fieldcollection/
---
## ResourceUsageView.FieldCollection property

Gets the [`ResourceUsageViewFieldCollection`](../../resourceusageviewfieldcollection/) object of this ResourceUsageView.

```csharp
public ResourceUsageViewFieldCollection FieldCollection { get; }
```

## Examples

Shows how to read resource usage view fields.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### See Also

* class [ResourceUsageViewFieldCollection](../../resourceusageviewfieldcollection/)
* class [ResourceUsageView](../)
* namespace [Aspose.Tasks](../../resourceusageview/)
* assembly [Aspose.Tasks](../../../)


