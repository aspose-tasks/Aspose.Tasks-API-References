---
title: "IVbaModule.SourceCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "IVbaModule eigenschap. Haalt de broncode van de VBA-module op"
type: docs
weight: 30
url: /nl/net/aspose.tasks/ivbamodule/sourcecode/
---
## IVbaModule.SourceCode property

Haalt de broncode van de VBA‑module op

```csharp
public string SourceCode { get; }
```

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

* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


