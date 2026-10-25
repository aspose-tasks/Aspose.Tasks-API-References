---
title: "VbaModuleAttribute.Value"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "VbaModuleAttribute property. Ottiene il valore dell'attributo del modulo VBA"
type: docs
weight: 20
url: /it/net/aspose.tasks/vbamoduleattribute/value/
---
## VbaModuleAttribute.Value property

Ottiene il valore dell'attributo del modulo VBA.

```csharp
public string Value { get; }
```

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

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


