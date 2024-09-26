---
title: VbaProject.HelpFile
second_title: Aspose.Tasks for .NET API Reference
description: VbaProject property. Gets a help file name
type: docs
weight: 40
url: /net/aspose.tasks/vbaproject/helpfile/
---
## VbaProject.HelpFile property

Gets a help file name

```csharp
public string HelpFile { get; }
```

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

* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


