---
title: "Interfaccia IVbaModule"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Interfaccia Aspose.Tasks.IVbaModule. Rappresenta un modulo con codice VBA"
type: docs
weight: 880
url: /it/net/aspose.tasks/ivbamodule/
---
## IVbaModule interface

Rappresenta un modulo con codice VBA.

```csharp
public interface IVbaModule
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Attributes](../../aspose.tasks/ivbamodule/attributes/) { get; } | Ottiene una collezione di [`VbaModuleAttributeCollection`](../vbamoduleattributecollection/) |
| [Name](../../aspose.tasks/ivbamodule/name/) { get; } | Ottiene il nome del modulo VBA |
| [SourceCode](../../aspose.tasks/ivbamodule/sourcecode/) { get; } | Ottiene il codice sorgente del modulo VBA |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


