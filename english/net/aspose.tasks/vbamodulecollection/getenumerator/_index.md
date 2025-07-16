---
title: VbaModuleCollection.GetEnumerator
second_title: Aspose.Tasks for .NET API Reference
description: VbaModuleCollection method. 
type: docs
weight: 80
url: /net/aspose.tasks/vbamodulecollection/getenumerator/
---
## VbaModuleCollection.GetEnumerator method

```csharp
public IEnumerator<VbaModule> GetEnumerator()
```

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


