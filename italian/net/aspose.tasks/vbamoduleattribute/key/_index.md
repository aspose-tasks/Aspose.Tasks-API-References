---
title: "VbaModuleAttribute.Key"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà VbaModuleAttribute. Ottiene la chiave dell'attributo del modulo VBA"
type: docs
weight: 10
url: /it/net/aspose.tasks/vbamoduleattribute/key/
---
## VbaModuleAttribute.Key property

Ottiene la chiave dell'attributo del modulo VBA.

```csharp
public string Key { get; }
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


