---
title: VbaProject.Modules
second_title: Aspose.Tasks for .NET API Reference
description: VbaProject property. Gets a collection of VbaModuleCollection
type: docs
weight: 50
url: /net/aspose.tasks/vbaproject/modules/
---
## VbaProject.Modules property

Gets a collection of [`VbaModuleCollection`](../../vbamodulecollection/)

```csharp
public VbaModuleCollection Modules { get; }
```

## Examples

Shows how to iterate over VBS modules of the project.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### See Also

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


