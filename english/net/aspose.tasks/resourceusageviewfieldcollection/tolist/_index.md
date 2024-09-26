---
title: ResourceUsageViewFieldCollection.ToList
second_title: Aspose.Tasks for .NET API Reference
description: ResourceUsageViewFieldCollection method. Converts the instance of the ResourceUsageViewFieldCollection class to a list containing the instances of the ResourceUsageViewField class
type: docs
weight: 20
url: /net/aspose.tasks/resourceusageviewfieldcollection/tolist/
---
## ResourceUsageViewFieldCollection.ToList method

Converts the instance of the [`ResourceUsageViewFieldCollection`](../) class to a list containing the instances of the [`ResourceUsageViewField`](../../resourceusageviewfield/) class.

```csharp
public IList<ResourceUsageViewField> ToList()
```

### Return Value

The instance of the [`ResourceUsageViewFieldCollection`](../) class converted to list containing the instances of the [`ResourceUsageViewField`](../../resourceusageviewfield/) class.

## Examples

Shows how to work field collection of a ResourceUsageView instance.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// one can transform collection into a list of ResourceUsageViewField
IList<ResourceUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### See Also

* enum [ResourceUsageViewField](../../resourceusageviewfield/)
* class [ResourceUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../resourceusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


