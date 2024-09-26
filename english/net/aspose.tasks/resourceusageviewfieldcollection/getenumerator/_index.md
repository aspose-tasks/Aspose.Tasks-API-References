---
title: ResourceUsageViewFieldCollection.GetEnumerator
second_title: Aspose.Tasks for .NET API Reference
description: ResourceUsageViewFieldCollection method. Returns an enumerator for this collection
type: docs
weight: 10
url: /net/aspose.tasks/resourceusageviewfieldcollection/getenumerator/
---
## ResourceUsageViewFieldCollection.GetEnumerator method

Returns an enumerator for this collection.

```csharp
public IEnumerator<ResourceUsageViewField> GetEnumerator()
```

### Return Value

an enumerator for this collection.

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


