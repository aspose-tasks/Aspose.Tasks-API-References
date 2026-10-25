---
title: "VbaModule.Attributes"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "VbaModule eigenschap. Haalt een collectie van de attributen van de module op"
type: docs
weight: 30
url: /nl/net/aspose.tasks/vbamodule/attributes/
---
## VbaModule.Attributes property

Haalt een verzameling van de attributen van de module op.

```csharp
public VbaModuleAttributeCollection Attributes { get; }
```

## Voorbeelden

Toont hoe de attributen van een VBA-module gelezen kunnen worden.

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

### Zie ook

* class [VbaModuleAttributeCollection](../../vbamoduleattributecollection/)
* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


