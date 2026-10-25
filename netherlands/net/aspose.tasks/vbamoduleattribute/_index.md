---
title: "Class VbaModuleAttribute"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.VbaModuleAttribute‑klasse. Het attribuut van het VbaModule‑object"
type: docs
weight: 2820
url: /nl/net/aspose.tasks/vbamoduleattribute/
---
## VbaModuleAttribute class

Het attribuut van het [`VbaModule`](../vbamodule/)‑object

```csharp
public sealed class VbaModuleAttribute : IEquatable<VbaModuleAttribute>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Key](../../aspose.tasks/vbamoduleattribute/key/) { get; } | Haalt de sleutel van het VBA‑module‑attribuut op. |
| [Value](../../aspose.tasks/vbamoduleattribute/value/) { get; } | Haalt de waarde van het VBA‑module‑attribuut op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals_1)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven `VbaModuleAttribute` object. |
| [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals)(VbaModuleAttribute) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven `VbaModuleAttribute` object. |
| override [GetHashCode](../../aspose.tasks/vbamoduleattribute/gethashcode/)() | Retourneert een hashcodewaarde voor dit `VbaModuleAttribute`. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


