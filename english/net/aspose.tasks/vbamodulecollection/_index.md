---
title: Class VbaModuleCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.VbaModuleCollection class. Represents a collection of VbaModule objects
type: docs
weight: 2760
url: /net/aspose.tasks/vbamodulecollection/
---
## VbaModuleCollection class

Represents a collection of [`VbaModule`](../vbamodule/) objects.

```csharp
public class VbaModuleCollection : ReadOnlyCollectionBase<VbaModule>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaModule) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

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

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaModule](../vbamodule/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


