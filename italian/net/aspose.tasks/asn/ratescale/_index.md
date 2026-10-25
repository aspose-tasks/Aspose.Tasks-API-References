---
title: "Asn.RateScale"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. L'unità di tempo per il tasso di utilizzo dell'assegnazione della risorsa materiale. Restituisce 0 se non definita"
type: docs
weight: 410
url: /it/net/aspose.tasks/asn/ratescale/
---
## Asn.RateScale field

L'unità di tempo per il tasso di utilizzo dell'assegnazione della risorsa materiale. Restituisce 0 se non definita.

```csharp
public static readonly Key<RateScaleType, AsnKey> RateScale;
```

## Esempi

Mostra come lavorare con la scala di tariffa dell'assegnazione quando vogliamo impostare un consumo materiale variabile (ad es. '10/day' o '1/week') per un'assegnazione di una risorsa materiale.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var nonMaterialResource = project.Resources.Add("nonMaterialResource");
nonMaterialResource.Set(Rsc.Type, ResourceType.Work);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Supponiamo di voler impostare il consumo materiale '1/week'.
// Dovremmo impostare la tariffa oraria nella proprietà Units, quindi dividiamo 1D per le ore settimanali.
materialResourceAssignment.Set(Asn.Units, 1D / 40);
materialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

// Nota che a partire dalla versione 24.4, questo può essere fatto chiamando un metodo:
// materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);

var nonMaterialResourceAssignment = project.ResourceAssignments.Add(task, nonMaterialResource);
nonMaterialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

project.Save(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp", SaveFileFormat.Mpp);

var resavedProject = new Project(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp");

var resavedMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(2);
Console.WriteLine(resavedMaterialResourceAssignment.Get(Asn.RateScale));

// Solo le assegnazioni di risorse materiali possono avere un valore di scala di tariffa diverso da zero.
var resavedNonMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(3);
Console.WriteLine(resavedNonMaterialResourceAssignment.Get(Asn.RateScale));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateScaleType](../../ratescaletype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


