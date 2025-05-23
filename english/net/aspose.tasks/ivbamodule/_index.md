---
title: Interface IVbaModule
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.IVbaModule interface. Represents a module with VBA code
type: docs
weight: 880
url: /net/aspose.tasks/ivbamodule/
---
## IVbaModule interface

Represents a module with VBA code.

```csharp
public interface IVbaModule
```

## Properties

| Name | Description |
| --- | --- |
| [Attributes](../../aspose.tasks/ivbamodule/attributes/) { get; } | Gets a collection of [`VbaModuleAttributeCollection`](../vbamoduleattributecollection/) |
| [Name](../../aspose.tasks/ivbamodule/name/) { get; } | Gets a name of the VBA module |
| [SourceCode](../../aspose.tasks/ivbamodule/sourcecode/) { get; } | Gets a source Code of the VBA module |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


