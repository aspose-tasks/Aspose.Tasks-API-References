---
title: "Asn.RateScale"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. De tijdseenheid voor de gebruikssnelheid van de materiaalresource-toewijzing. Retourneert 0 indien niet gedefinieerd"
type: docs
weight: 410
url: /nl/net/aspose.tasks/asn/ratescale/
---
## Asn.RateScale field

De tijdseenheid voor het gebruikstarief van de materiële resource-toewijzing. Retourneert 0 indien niet gedefinieerd.

```csharp
public static readonly Key<RateScaleType, AsnKey> RateScale;
```

## Voorbeelden

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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateScaleType](../../ratescaletype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


