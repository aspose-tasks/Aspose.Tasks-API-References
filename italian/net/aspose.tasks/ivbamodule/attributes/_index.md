---
title: "IVbaModule.Attributes"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà IVbaModule. Ottiene una raccolta di VbaModuleAttributeCollection"
type: docs
weight: 10
url: /it/net/aspose.tasks/ivbamodule/attributes/
---
## IVbaModule.Attributes property

Ottiene una raccolta di [`VbaModuleAttributeCollection`](../../vbamoduleattributecollection/)

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
* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


