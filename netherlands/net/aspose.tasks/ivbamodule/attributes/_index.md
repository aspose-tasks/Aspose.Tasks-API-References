---
title: "IVbaModule.Attributes"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "IVbaModule eigenschap. Haalt een collectie van VbaModuleAttributeCollection op"
type: docs
weight: 10
url: /nl/net/aspose.tasks/ivbamodule/attributes/
---
## IVbaModule.Attributes property

Haalt een collectie van [`VbaModuleAttributeCollection`](../../vbamoduleattributecollection/) op

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
* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


