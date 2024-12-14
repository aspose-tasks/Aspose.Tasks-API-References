---
title: Project.VbaProject
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets an instance of VbaProject class
type: docs
weight: 1000
url: /net/aspose.tasks/project/vbaproject/
---
## Project.VbaProject property

Gets an instance of `VbaProject` class.

```csharp
public VbaProject VbaProject { get; }
```

## Examples

Shows how to remove VBA macros from MPP file.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

Shows how to read VBA project information.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

### See Also

* class [VbaProject](../../vbaproject/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


