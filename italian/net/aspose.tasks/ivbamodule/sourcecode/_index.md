---
title: "IVbaModule.SourceCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà IVbaModule. Ottiene il codice sorgente del modulo VBA"
type: docs
weight: 30
url: /it/net/aspose.tasks/ivbamodule/sourcecode/
---
## IVbaModule.SourceCode property

Ottiene il codice sorgente del modulo VBA

```csharp
public string SourceCode { get; }
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

* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


