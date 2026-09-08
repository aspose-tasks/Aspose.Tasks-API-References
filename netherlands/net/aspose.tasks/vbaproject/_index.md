---
title: "Klasse VbaProject"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.VbaProject klasse. Vertegenwoordigt VbaProject"
type: docs
weight: 2860
url: /nl/net/aspose.tasks/vbaproject/
---
## VbaProject class

Vertegenwoordigt `VbaProject`.

```csharp
public class VbaProject
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CompilationArguments](../../aspose.tasks/vbaproject/compilationarguments/) { get; } | Haalt voorwaardelijke compilatie‑argumenten op |
| [Description](../../aspose.tasks/vbaproject/description/) { get; } | Haalt een projectbeschrijving op. |
| [HelpContextId](../../aspose.tasks/vbaproject/helpcontextid/) { get; } | Haalt een project Help Context Id op |
| [HelpFile](../../aspose.tasks/vbaproject/helpfile/) { get; } | Haalt een helpbestandsnaam op |
| [Modules](../../aspose.tasks/vbaproject/modules/) { get; } | Haalt een collectie op van [`VbaModuleCollection`](../vbamodulecollection/) |
| [Name](../../aspose.tasks/vbaproject/name/) { get; } | Haalt projectnaam op |
| [References](../../aspose.tasks/vbaproject/references/) { get; } | Haalt een collectie op van [`VbaReferenceCollection`](../vbareferencecollection/) |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


