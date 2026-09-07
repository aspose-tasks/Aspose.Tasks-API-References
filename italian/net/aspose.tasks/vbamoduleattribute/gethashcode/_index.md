---
title: "VbaModuleAttribute.GetHashCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo VbaModuleAttribute. Restituisce un valore di hash code per questo VbaModuleAttribute"
type: docs
weight: 40
url: /it/net/aspose.tasks/vbamoduleattribute/gethashcode/
---
## VbaModuleAttribute.GetHashCode method

Restituisce un valore di hash code per questo [`VbaModuleAttribute`](../).

```csharp
public override int GetHashCode()
```

### Valore di ritorno

Restituisce un valore di hash code per questo oggetto.

## Esempi

Mostra come ottenere un hash code di un attributo del modulo VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];

// stampa gli hash code di attributi del modulo VBA
Console.WriteLine("Hash codes of VBA module attributes are based on key and value hash codes.");
Console.WriteLine("VBA module attribute 1 Hash Code: {0}", attribute1.GetHashCode());
Console.WriteLine("VBA module attribute 2 Hash Code: {0}", attribute2.GetHashCode());
```

### Vedi anche

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


