---
title: "VbaModule.Name"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "VbaModule eigenschap. Haalt de naam van de VBA-module op"
type: docs
weight: 40
url: /nl/net/aspose.tasks/vbamodule/name/
---
## VbaModule.Name property

Haalt een naam van de VBA-module op

```csharp
public string Name { get; set; }
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

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


