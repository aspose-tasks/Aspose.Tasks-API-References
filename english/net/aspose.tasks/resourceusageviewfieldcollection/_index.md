---
title: Class ResourceUsageViewFieldCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ResourceUsageViewFieldCollection class. Represent a collection of ResourceUsageViewField values
type: docs
weight: 1770
url: /net/aspose.tasks/resourceusageviewfieldcollection/
---
## ResourceUsageViewFieldCollection class

Represent a collection of [`ResourceUsageViewField`](../resourceusageviewfield/) values.

```csharp
public class ResourceUsageViewFieldCollection : IList<ResourceUsageViewField>
```

## Methods

| Name | Description |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/resourceusageviewfieldcollection/getenumerator/)() | Returns an enumerator for this collection. |
| [ToList](../../aspose.tasks/resourceusageviewfieldcollection/tolist/)() | Converts the instance of the `ResourceUsageViewFieldCollection` class to a list containing the instances of the [`ResourceUsageViewField`](../resourceusageviewfield/) class. |

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

* enum [ResourceUsageViewField](../resourceusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


