---
title: "Interface IVbaModule"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.IVbaModule interface. Stelt een module met VBA‑code voor"
type: docs
weight: 880
url: /nl/net/aspose.tasks/ivbamodule/
---
## IVbaModule interface

Stelt een module met VBA‑code voor.

```csharp
public interface IVbaModule
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Attributes](../../aspose.tasks/ivbamodule/attributes/) { get; } | Haalt een collectie van [`VbaModuleAttributeCollection`](../vbamoduleattributecollection/) op |
| [Name](../../aspose.tasks/ivbamodule/name/) { get; } | Haalt een naam van de VBA-module op |
| [SourceCode](../../aspose.tasks/ivbamodule/sourcecode/) { get; } | Haalt de broncode van de VBA‑module op |

## Voorbeelden

Toont hoe modules van een VBA-project gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


