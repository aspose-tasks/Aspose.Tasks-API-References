---
title: "VbaModule.Attributes"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà VbaModule. Ottiene una collezione degli attributi del modulo"
type: docs
weight: 30
url: /it/net/aspose.tasks/vbamodule/attributes/
---
## VbaModule.Attributes property

Ottiene una raccolta degli attributi del modulo.

```csharp
public VbaModuleAttributeCollection Attributes { get; }
```

## Esempi

Mostra come leggere gli attributi del modulo VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("VB Name: " + attribute.Key);
        Console.WriteLine("Module: " + attribute.Value);
    }
}
```

### Vedi anche

* class [VbaModuleAttributeCollection](../../vbamoduleattributecollection/)
* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


