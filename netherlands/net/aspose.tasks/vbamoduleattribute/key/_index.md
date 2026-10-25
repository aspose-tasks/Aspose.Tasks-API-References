---
title: "VbaModuleAttribute.Key"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "VbaModuleAttribute eigenschap. Haalt de sleutel van VBA-module-attribuut op"
type: docs
weight: 10
url: /nl/net/aspose.tasks/vbamoduleattribute/key/
---
## VbaModuleAttribute.Key property

Haalt de sleutel van het VBA‑module‑attribuut op.

```csharp
public string Key { get; }
```

## Voorbeelden

Toont hoe te werken met VBA-module-attributen.

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

### Zie ook

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


