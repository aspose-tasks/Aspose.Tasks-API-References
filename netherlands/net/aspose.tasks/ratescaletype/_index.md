---
title: "Enum RateScaleType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.RateScaleType enum. Specificeert het tariefschaaltype"
type: docs
weight: 1650
url: /nl/net/aspose.tasks/ratescaletype/
---
## RateScaleType enumeration

Specificeert het type tariefschaal.

```csharp
public enum RateScaleType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `0` | Geeft een ongedefinieerd tariefschaaltype aan. |
| Minute | `1` | Geeft een minuut tariefschaaltype aan. |
| Hour | `2` | Geeft een uur tariefschaaltype aan. |
| Day | `3` | Geeft een dag tariefschaaltype aan. |
| Week | `4` | Geeft een week tariefschaaltype aan. |
| Month | `5` | Geeft een maand tariefschaaltype aan. |
| Quarter | `6` | Geeft een kwartaal tariefschaaltype aan. |
| Year | `7` | Geeft een jaar tariefschaaltype aan. |

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

Toont hoe te werken met de tariefschaal van een toewijzing wanneer we variabele materiaalconsumptie (bijv. '10/day' of '1/week') voor een toewijzing van een materiaalresource willen instellen.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var nonMaterialResource = project.Resources.Add("nonMaterialResource");
nonMaterialResource.Set(Rsc.Type, ResourceType.Work);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Stel dat we de materiaalconsumptie op '1/week' willen instellen.
// We moeten het uurtarief instellen op de Units-eigenschap, zodat we 1D delen door uren per week.
materialResourceAssignment.Set(Asn.Units, 1D / 40);
materialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

// Let op dat vanaf 24.4 dit kan worden gedaan door één methode aan te roepen:
// materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);

var nonMaterialResourceAssignment = project.ResourceAssignments.Add(task, nonMaterialResource);
nonMaterialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

project.Save(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp", SaveFileFormat.Mpp);

var resavedProject = new Project(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp");

var resavedMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(2);
Console.WriteLine(resavedMaterialResourceAssignment.Get(Asn.RateScale));

// Alleen materiaalresource-toewijzingen kunnen een niet-nul tariefschaalwaarde hebben.
var resavedNonMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(3);
Console.WriteLine(resavedNonMaterialResourceAssignment.Get(Asn.RateScale));
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


