---
title: Class VbaModule
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.VbaModule class. Represents a VBA module
type: docs
weight: 2790
url: /net/aspose.tasks/vbamodule/
---
## VbaModule class

Represents a VBA module.

```csharp
public sealed class VbaModule
```

## Properties

| Name | Description |
| --- | --- |
| [Attributes](../../aspose.tasks/vbamodule/attributes/) { get; } | Gets a collection of the module's attributes. |
| [Name](../../aspose.tasks/vbamodule/name/) { get; set; } | Gets a name of the VBA module |
| [SourceCode](../../aspose.tasks/vbamodule/sourcecode/) { get; set; } | Gets or sets a source code of the VBA module |
| [Type](../../aspose.tasks/vbamodule/type/) { get; } | Gets the type of the module. |

## Methods

| Name | Description |
| --- | --- |
| static [CreateClassModule](../../aspose.tasks/vbamodule/createclassmodule/)(string) | Creates an instance of `VbaModule` with VbaModuleType.ClassModule type. |
| static [CreateProceduralModule](../../aspose.tasks/vbamodule/createproceduralmodule/)(string) | Creates an instance of `VbaModule` with VbaModuleType.ProceduralModule type. |

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


