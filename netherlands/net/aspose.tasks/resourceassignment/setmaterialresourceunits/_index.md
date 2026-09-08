---
title: "ResourceAssignment.SetMaterialResourceUnits"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment‑methode. Stelt eenheden in voor de toewijzing van een materiële resource met variabele materiaalconsumptie. De variabele materiaalconsumptie betekent dat naarmate de toewijzingsduur verandert, de hoeveelheid gebruikte materialen evenredig verandert."
type: docs
weight: 760
url: /nl/net/aspose.tasks/resourceassignment/setmaterialresourceunits/
---
## ResourceAssignment.SetMaterialResourceUnits method

Stelt eenheden in voor de toewijzing van een materiële resource met variabele materiaalconsumptie. Variabele materiaalconsumptie betekent dat naarmate de toewijzingsduur verandert, de hoeveelheid gebruikte materialen evenredig verandert.

```csharp
public void SetMaterialResourceUnits(double units, RateScaleType rateScaleType)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| eenheden | Double | Aantal eenheden dat is opgebouwd gedurende de tijdsperiode. |
| rateScaleType | RateScaleType | Tijdsperiode waarin de eenheidswaarde wordt opgebouwd. |

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| InvalidOperationException | Als de methode wordt aangeroepen voor de toewijzing van een niet-materiële resource. |

## Opmerkingen

Bijvoorbeeld, om '123/maand' in te stellen, moet SetUnitsScaled(123D, RateScaleType.Month) worden aangeroepen.

## Voorbeelden

Toont hoe variabele materiaalconsumptie (bijv. '10/day' of '1/week') in te stellen voor een toewijzing van een materiaalresource.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Stel dat we de materiaalconsumptie op '1/week' willen instellen.
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

### Zie ook

* enum [RateScaleType](../../ratescaletype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


