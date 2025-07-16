---
title: VbaModuleCollection.ToList
second_title: Aspose.Tasks for .NET API Reference
description: VbaModuleCollection method. Converts the collection object to a list of VbaModule objects
type: docs
weight: 100
url: /net/aspose.tasks/vbamodulecollection/tolist/
---
## VbaModuleCollection.ToList method

Converts the collection object to a list of [`VbaModule`](../../vbamodule/) objects.

```csharp
public List<VbaModule> ToList()
```

### Return Value

List of objects.

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

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


