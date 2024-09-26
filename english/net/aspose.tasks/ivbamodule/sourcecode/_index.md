---
title: IVbaModule.SourceCode
second_title: Aspose.Tasks for .NET API Reference
description: IVbaModule property. Gets a source Code of the VBA module
type: docs
weight: 30
url: /net/aspose.tasks/ivbamodule/sourcecode/
---
## IVbaModule.SourceCode property

Gets a source Code of the VBA module

```csharp
public string SourceCode { get; }
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


