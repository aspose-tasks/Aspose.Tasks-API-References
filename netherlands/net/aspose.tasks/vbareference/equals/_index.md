---
title: "VbaReference.Equals"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "VbaReference-methode. Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven VbaReference-object"
type: docs
weight: 40
url: /nl/net/aspose.tasks/vbareference/equals/
---
## Equals(VbaReference) {#equals}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven [`VbaReference`](../)-object.

```csharp
public bool Equals(VbaReference other)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | VbaReference | Het opgegeven [`VbaReference`](../)-object om te vergelijken met deze instantie. |

### Retourwaarde

Retourneert true als deze instantie gelijk is aan het opgegeven [`VbaReference`](../)-object; anders false.

## Voorbeelden

Toont hoe je VBA-referentie‑gelijkheid controleert.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// De gelijkheid van referenties wordt gecontroleerd aan de hand van de naam van de referentie.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### Zie ook

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven [`VbaReference`](../)-object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | Object | Het opgegeven [`VbaReference`](../)-object om te vergelijken met deze instantie. |

### Retourwaarde

Retourneert true als deze instantie gelijk is aan het opgegeven [`VbaReference`](../)-object; anders false.

## Voorbeelden

Toont hoe je VBA-referentie‑gelijkheid controleert.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// De gelijkheid van referenties wordt gecontroleerd aan de hand van de naam van de referentie.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### Zie ook

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


