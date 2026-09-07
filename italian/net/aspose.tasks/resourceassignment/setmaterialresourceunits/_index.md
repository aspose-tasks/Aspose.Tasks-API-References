---
title: "ResourceAssignment.SetMaterialResourceUnits"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ResourceAssignment. Imposta le unità per l'assegnazione di una risorsa materiale con consumo variabile di materiale. Il consumo variabile di materiale significa che, man mano che la durata dell'assegnazione cambia, la quantità di materiali utilizzati varia proporzionalmente."
type: docs
weight: 760
url: /it/net/aspose.tasks/resourceassignment/setmaterialresourceunits/
---
## ResourceAssignment.SetMaterialResourceUnits method

Imposta le unità per l'assegnazione di una risorsa materiale con consumo variabile di materiale. Il consumo variabile di materiale significa che, al variare della durata dell'assegnazione, la quantità di materiali utilizzati cambia proporzionalmente.

```csharp
public void SetMaterialResourceUnits(double units, RateScaleType rateScaleType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| unità | Double | Numero di unità accumulate nel periodo di tempo. |
| rateScaleType | RateScaleType | Periodo di tempo in cui il valore dell'unità è accumulato. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Se il metodo è chiamato per l'assegnazione di una risorsa non materiale. |

## Osservazioni

Ad esempio, per impostare '123/mese', dovrebbe essere chiamato SetUnitsScaled(123D, RateScaleType.Month).

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

### Vedi anche

* enum [RateScaleType](../../ratescaletype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


