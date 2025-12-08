---
title: Class VbaModuleCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.VbaModuleCollection class. Represents a collection of VbaModule objects
type: docs
weight: 2790
url: /net/aspose.tasks/vbamodulecollection/
---
## VbaModuleCollection class

Represents a collection of [`VbaModule`](../vbamodule/) objects.

```csharp
public class VbaModuleCollection : ICollection<VbaModule>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/vbamodulecollection/count/) { get; } |  |
| [IsReadOnly](../../aspose.tasks/vbamodulecollection/isreadonly/) { get; } |  |
| [Item](../../aspose.tasks/vbamodulecollection/item/) { get; } | Gets the module at the specified index. (2 indexers) |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/vbamodulecollection/add/)(VbaModule) |  |
| [Clear](../../aspose.tasks/vbamodulecollection/clear/)() |  |
| [Contains](../../aspose.tasks/vbamodulecollection/contains/)(VbaModule) |  |
| [CopyTo](../../aspose.tasks/vbamodulecollection/copyto/)(VbaModule[], int) |  |
| [GetEnumerator](../../aspose.tasks/vbamodulecollection/getenumerator/)() |  |
| [Remove](../../aspose.tasks/vbamodulecollection/remove/)(VbaModule) |  |
| [ToList](../../aspose.tasks/vbamodulecollection/tolist/)() | Converts the collection object to a list of [`VbaModule`](../vbamodule/) objects. |

## Examples

Shows how to iterate over VBA modules.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var vbaProject = project.VbaProject;

Console.WriteLine("Total Modules Count: " + vbaProject.Modules.Count);
foreach (VbaModule module in vbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Module Type: " + module.Type);
    Console.WriteLine("Source Code: " + module.SourceCode);
    Console.WriteLine();
}
```

### See Also

* class [VbaModule](../vbamodule/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


