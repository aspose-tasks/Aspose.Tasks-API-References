---
title: "IVbaModule.Name"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "IVbaModule eigenschap. Haalt een naam van de VBA-module op"
type: docs
weight: 20
url: /nl/net/aspose.tasks/ivbamodule/name/
---
## IVbaModule.Name property

Haalt een naam van de VBA-module op

```csharp
public string Name { get; }
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


