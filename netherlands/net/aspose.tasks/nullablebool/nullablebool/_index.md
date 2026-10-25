---
title: "NullableBool.NullableBool"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "NullableBool-constructor. Initialiseert een nieuwe instantie van de NullableBool-struct met de opgegeven booleaanse waarde"
type: docs
weight: 10
url: /nl/net/aspose.tasks/nullablebool/nullablebool/
---
## NullableBool(bool) {#constructor}

Initialiseert een nieuwe instantie van de [`NullableBool`](../)‑struct met de opgegeven booleaanse waarde.

```csharp
public NullableBool(bool value)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | Boolean | de gespecificeerde booleaanse waarde. |

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

---

## NullableBool(bool, bool) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`NullableBool`](../) struct.

```csharp
public NullableBool(bool value, bool isDefined)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | Boolean | De huidige waarde. |
| isDefined | Boolean | De waarde die aangeeft of de huidige waarde is gedefinieerd. |

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


