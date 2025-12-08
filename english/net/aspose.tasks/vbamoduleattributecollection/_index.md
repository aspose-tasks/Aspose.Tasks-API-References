---
title: Class VbaModuleAttributeCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.VbaModuleAttributeCollection class. Represents a collection of VbaModuleAttribute objects
type: docs
weight: 2780
url: /net/aspose.tasks/vbamoduleattributecollection/
---
## VbaModuleAttributeCollection class

Represents a collection of [`VbaModuleAttribute`](../vbamoduleattribute/) objects.

```csharp
public class VbaModuleAttributeCollection : ReadOnlyCollectionBase<VbaModuleAttribute>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaModuleAttribute) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## Examples

Shows how to iterate over VBA module's attribute collection.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("Attribute Name: " + attribute.Key);
        Console.WriteLine("Attribute Value: " + attribute.Value);
    }
}
```

### See Also

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaModuleAttribute](../vbamoduleattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


