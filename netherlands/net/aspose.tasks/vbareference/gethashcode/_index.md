---
title: "VbaReference.GetHashCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "VbaReference-methode. Retourneert een hashcode‑waarde voor deze VbaReference"
type: docs
weight: 50
url: /nl/net/aspose.tasks/vbareference/gethashcode/
---
## VbaReference.GetHashCode method

Retourneert een hashcode‑waarde voor deze [`VbaReference`](../).

```csharp
public override int GetHashCode()
```

### Retourwaarde

Retourneert een hashcode‑waarde voor dit object.

## Voorbeelden

Toont hoe je een hashcode van een VBA-referentie krijgt.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// De hashcode van een referentie is een hashcode van de GUID van de interne referentie
Console.WriteLine("VBA reference Hash Code: {0}", reference1.GetHashCode());
Console.WriteLine("VBA reference Hash Code: {0}", reference2.GetHashCode());
```

### Zie ook

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


