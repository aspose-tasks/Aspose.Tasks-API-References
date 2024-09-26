---
title: IVbaModule.Name
second_title: Aspose.Tasks for .NET API Reference
description: IVbaModule property. Gets a name of the VBA module
type: docs
weight: 20
url: /net/aspose.tasks/ivbamodule/name/
---
## IVbaModule.Name property

Gets a name of the VBA module

```csharp
public string Name { get; }
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

* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


