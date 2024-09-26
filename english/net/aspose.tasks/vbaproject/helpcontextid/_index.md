---
title: VbaProject.HelpContextId
second_title: Aspose.Tasks for .NET API Reference
description: VbaProject property. Gets a project Help Context Id
type: docs
weight: 30
url: /net/aspose.tasks/vbaproject/helpcontextid/
---
## VbaProject.HelpContextId property

Gets a project Help Context Id

```csharp
public int HelpContextId { get; }
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


