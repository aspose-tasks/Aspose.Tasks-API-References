---
title: "VbaProject.HelpFile"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "VbaProject-eigenschap. Haalt een helpbestandsnaam op"
type: docs
weight: 40
url: /nl/net/aspose.tasks/vbaproject/helpfile/
---
## VbaProject.HelpFile property

Haalt een helpbestandsnaam op

```csharp
public string HelpFile { get; }
```

## Voorbeelden

Toont hoe VBA-projecteigenschappen te lezen.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

### Zie ook

* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


