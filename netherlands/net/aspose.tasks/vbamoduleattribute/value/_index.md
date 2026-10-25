---
title: "VbaModuleAttribute.Value"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "VbaModuleAttribute property. Haalt de waarde van het VBA‑module‑attribuut op"
type: docs
weight: 20
url: /nl/net/aspose.tasks/vbamoduleattribute/value/
---
## VbaModuleAttribute.Value property

Haalt de waarde van het VBA‑module‑attribuut op.

```csharp
public string Value { get; }
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


