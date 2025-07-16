---
title: VbaModule.Name
second_title: Aspose.Tasks for .NET API Reference
description: VbaModule property. Gets a name of the VBA module
type: docs
weight: 40
url: /net/aspose.tasks/vbamodule/name/
---
## VbaModule.Name property

Gets a name of the VBA module

```csharp
public string Name { get; set; }
```

## Examples

Shows how to read modules of VBA project.

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

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


