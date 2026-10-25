---
title: "Classe VbaModuleAttribute"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.VbaModuleAttribute. L'attributo dell'oggetto VbaModule"
type: docs
weight: 2820
url: /it/net/aspose.tasks/vbamoduleattribute/
---
## VbaModuleAttribute class

L'attributo dell'oggetto [`VbaModule`](../vbamodule/)

```csharp
public sealed class VbaModuleAttribute : IEquatable<VbaModuleAttribute>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Key](../../aspose.tasks/vbamoduleattribute/key/) { get; } | Ottiene la chiave dell'attributo del modulo VBA. |
| [Value](../../aspose.tasks/vbamoduleattribute/value/) { get; } | Ottiene il valore dell'attributo del modulo VBA. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals_1)(object) | Restituisce un valore che indica se questa istanza è uguale all'oggetto `VbaModuleAttribute` specificato. |
| [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals)(VbaModuleAttribute) | Restituisce un valore che indica se questa istanza è uguale all'oggetto `VbaModuleAttribute` specificato. |
| override [GetHashCode](../../aspose.tasks/vbamoduleattribute/gethashcode/)() | Restituisce un valore di codice hash per questo `VbaModuleAttribute`. |

## Esempi

Mostra come lavorare con gli attributi del modulo VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("  VB Name: " + attribute.Key);
        Console.WriteLine("  Module: " + attribute.Value);
    }
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


