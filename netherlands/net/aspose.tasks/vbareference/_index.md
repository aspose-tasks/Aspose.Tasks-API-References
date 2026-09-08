---
title: "Klasse VbaReference"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.VbaReference klasse. Vertegenwoordigt een referentie van het VbaProject"
type: docs
weight: 2870
url: /nl/net/aspose.tasks/vbareference/
---
## VbaReference class

Stelt een referentie voor van de [`VbaProject`](../vbaproject/).

```csharp
public sealed class VbaReference : IEquatable<VbaReference>
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [VbaReference](vbareference/)() | De standaardconstructor. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [LibIdentifier](../../aspose.tasks/vbareference/libidentifier/) { get; } | Haalt de identifier van de bibliotheek op. |
| [Name](../../aspose.tasks/vbareference/name/) { get; set; } | Haalt de naam van de VBA-referentie op of stelt deze in. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [Equals](../../aspose.tasks/vbareference/equals/#equals_1)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven `VbaReference`-object. |
| [Equals](../../aspose.tasks/vbareference/equals/#equals)(VbaReference) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven `VbaReference`-object. |
| override [GetHashCode](../../aspose.tasks/vbareference/gethashcode/)() | Retourneert een hashcode-waarde voor dit `VbaReference`. |

## Voorbeelden

Toont hoe VBA-referenties gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


