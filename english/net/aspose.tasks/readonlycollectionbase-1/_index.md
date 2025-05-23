---
title: Class ReadOnlyCollectionBaseT
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ReadOnlyCollectionBase1T class. Represents a readonly collection of objects
type: docs
weight: 1610
url: /net/aspose.tasks/readonlycollectionbase-1/
---
## ReadOnlyCollectionBase&lt;T&gt; class

Represents a read-only collection of objects.

```csharp
public abstract class ReadOnlyCollectionBase<T> : IList<T>
```

| Parameter | Description |
| --- | --- |
| T | Type of collection items. |

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } | Gets the number of objects contained in the object. |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } | Returns the element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(T) | This is the stub implementation of ICollection's Add method, that only throws NotSupportedException |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() | Returns an enumerator for this collection. |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() | Converts the collection object to a list of [`VbaModule`](../vbamodule/) objects. |

## Examples

Shows how to iterate over VBA modules.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var vbaProject = project.VbaProject;

Console.WriteLine("Total Modules Count: " + vbaProject.Modules.Count);
foreach (var module in vbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
    Console.WriteLine();
}

// the collection can be converted into a plain list
List<VbaModule> modules = vbaProject.Modules.ToList();
foreach (var unused in modules)
{
    // work with modules
}
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


