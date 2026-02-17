---
title: Class VbaReferenceCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.VbaReferenceCollection class. Represents a collection of VbaReference objects
type: docs
weight: 2860
url: /net/aspose.tasks/vbareferencecollection/
---
## VbaReferenceCollection class

Represents a collection of [`VbaReference`](../vbareference/) objects.

```csharp
public class VbaReferenceCollection : ReadOnlyCollectionBase<VbaReference>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaReference) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## Examples

Shows how to work with VBA reference collection.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### See Also

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaReference](../vbareference/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


