---
title: "Struct NullableBool"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.NullableBool struct. Een klasse voor booleaanse waarden met de mogelijkheid te controleren of de waarde wel of niet is gedefinieerd."
type: docs
weight: 1110
url: /nl/net/aspose.tasks/nullablebool/
---
## NullableBool structure

Een klasse voor booleaanse waarden met de mogelijkheid te controleren of de waarde wel of niet gedefinieerd is.

```csharp
public struct NullableBool : IEquatable<NullableBool>
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [NullableBool](nullablebool/#constructor)(bool) | Initialiseert een nieuwe instantie van de `NullableBool` struct met de opgegeven booleaanse waarde. |
| [NullableBool](nullablebool/#constructor_1)(bool, bool) | Initialiseert een nieuwe instantie van de `NullableBool` struct. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [IsDefined](../../aspose.tasks/nullablebool/isdefined/) { get; } | Haalt een waarde op die aangeeft of de waarde gedefinieerd was; anders false. |
| [Value](../../aspose.tasks/nullablebool/value/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of de huidige waarde true of false is. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Equals](../../aspose.tasks/nullablebool/equals/#equals)(NullableBool) | Retourneert een vlag die aangeeft of deze instantie gelijk is aan de opgegeven instantie van de `NullableBool`-klasse. |
| override [Equals](../../aspose.tasks/nullablebool/equals/#equals_1)(object) | Retourneert een vlag die aangeeft of deze instantie gelijk is aan het opgegeven object. |
| override [GetHashCode](../../aspose.tasks/nullablebool/gethashcode/)() | Retourneert een hashcode-waarde voor de instantie van de `NullableBool`-klasse. |
| override [ToString](../../aspose.tasks/nullablebool/tostring/)() | Retourneert een string die het huidige object vertegenwoordigt. |
| [operator ==](../../aspose.tasks/nullablebool/op_equality/) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [implicit operator](../../aspose.tasks/nullablebool/op_implicit/#op_implicit_1) | Converteert impliciet een `NullableBool`-instantie naar een booleaanse waarde. Retourneert true wanneer [`Value`](./value/) true is en [`IsDefined`](./isdefined/) true is. (2 operatoren) |
| [operator !=](../../aspose.tasks/nullablebool/op_inequality/) | Retourneert een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object. |

## Voorbeelden

Toont hoe te werken met &lt;see cref="NullableBool" /&gt; klasse.

```csharp
var project = new Project();

// Laten we controleren waar de <see cref="Aspose.Tasks.NullableBool" /> klasse wordt gebruikt
// Het belangrijkste voordeel van <see cref="Aspose.Tasks.NullableBool" /> is dat 
// men kan het instellen als ongedefinieerd door constructie
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// gebruik nullable bool‑instantie
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// gebruik nullable bool‑instantie
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


