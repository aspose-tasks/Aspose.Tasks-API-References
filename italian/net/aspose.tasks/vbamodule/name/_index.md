---
title: "VbaModule.Name"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà VbaModule. Ottiene il nome del modulo VBA"
type: docs
weight: 40
url: /it/net/aspose.tasks/vbamodule/name/
---
## VbaModule.Name property

Ottiene il nome del modulo VBA

```csharp
public string Name { get; set; }
```

## Esempi

Mostra come leggere i moduli di un progetto VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### Vedi anche

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


