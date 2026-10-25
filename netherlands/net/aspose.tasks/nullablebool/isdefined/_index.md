---
title: "NullableBool.IsDefined"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "NullableBool-eigenschap. Haalt een waarde op die aangeeft of de waarde was gedefinieerd, anders false"
type: docs
weight: 20
url: /nl/net/aspose.tasks/nullablebool/isdefined/
---
## NullableBool.IsDefined property

Haalt een waarde op die aangeeft of de waarde gedefinieerd was; anders false.

```csharp
public bool IsDefined { get; }
```

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

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


