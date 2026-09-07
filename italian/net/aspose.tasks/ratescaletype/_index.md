---
title: "Enum RateScaleType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.RateScaleType. Specifica il tipo di scala di tariffa."
type: docs
weight: 1650
url: /it/net/aspose.tasks/ratescaletype/
---
## RateScaleType enumeration

Specifica il tipo di scala del tasso.

```csharp
public enum RateScaleType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `0` | Indica il tipo di scala di tariffa Undefined. |
| Minute | `1` | Indica il tipo di scala di tariffa Minute. |
| Hour | `2` | Indica il tipo di scala di tariffa Hour. |
| Day | `3` | Indica il tipo di scala di tariffa Day. |
| Week | `4` | Indica il tipo di scala di tariffa Week. |
| Month | `5` | Indica il tipo di scala di tariffa Month. |
| Quarter | `6` | Indica il tipo di scala di tariffa Quarter. |
| Year | `7` | Indica il tipo di scala di tariffa Year. |

## Esempi

Mostra come impostare il consumo materiale variabile (ad es. '10/day' o '1/week') per un'assegnazione di una risorsa materiale.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Supponiamo di voler impostare il consumo materiale '1/week'.
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


