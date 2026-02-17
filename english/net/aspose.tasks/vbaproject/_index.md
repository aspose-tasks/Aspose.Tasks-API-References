---
title: Class VbaProject
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.VbaProject class. Represents VbaProject
type: docs
weight: 2840
url: /net/aspose.tasks/vbaproject/
---
## VbaProject class

Represents `VbaProject`.

```csharp
public class VbaProject
```

## Properties

| Name | Description |
| --- | --- |
| [CompilationArguments](../../aspose.tasks/vbaproject/compilationarguments/) { get; } | Gets conditional Compilation Arguments |
| [Description](../../aspose.tasks/vbaproject/description/) { get; } | Gets a project description. |
| [HelpContextId](../../aspose.tasks/vbaproject/helpcontextid/) { get; } | Gets a project Help Context Id |
| [HelpFile](../../aspose.tasks/vbaproject/helpfile/) { get; } | Gets a help file name |
| [Modules](../../aspose.tasks/vbaproject/modules/) { get; } | Gets a collection of [`VbaModuleCollection`](../vbamodulecollection/) |
| [Name](../../aspose.tasks/vbaproject/name/) { get; } | Gets project name |
| [References](../../aspose.tasks/vbaproject/references/) { get; } | Gets a collection of [`VbaReferenceCollection`](../vbareferencecollection/) |

## Examples

Shows how to read VBA project properties.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


