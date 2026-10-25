---
title: "NullableBool.ToString"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "NullableBool-methode. Retourneert een string die het huidige object vertegenwoordigt"
type: docs
weight: 60
url: /nl/net/aspose.tasks/nullablebool/tostring/
---
## NullableBool.ToString method

Retourneert een string die het huidige object vertegenwoordigt.

```csharp
public override string ToString()
```

### Retourwaarde

Een string die het huidige object vertegenwoordigt.

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


