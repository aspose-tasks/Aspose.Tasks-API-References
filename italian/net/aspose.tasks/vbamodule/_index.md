---
title: "Classe VbaModule"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.VbaModule. Rappresenta un modulo VBA"
type: docs
weight: 2810
url: /it/net/aspose.tasks/vbamodule/
---
## VbaModule class

Rappresenta un modulo VBA.

```csharp
public sealed class VbaModule
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Attributes](../../aspose.tasks/vbamodule/attributes/) { get; } | Ottiene una raccolta degli attributi del modulo. |
| [Name](../../aspose.tasks/vbamodule/name/) { get; set; } | Ottiene il nome del modulo VBA |
| [SourceCode](../../aspose.tasks/vbamodule/sourcecode/) { get; set; } | Ottiene o imposta il codice sorgente del modulo VBA |
| [Type](../../aspose.tasks/vbamodule/type/) { get; } | Ottiene il tipo del modulo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CreateClassModule](../../aspose.tasks/vbamodule/createclassmodule/)(string) | Crea un'istanza di `VbaModule` con il tipo VbaModuleType.ClassModule. |
| static [CreateProceduralModule](../../aspose.tasks/vbamodule/createproceduralmodule/)(string) | Crea un'istanza di `VbaModule` con il tipo VbaModuleType.ProceduralModule. |

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


