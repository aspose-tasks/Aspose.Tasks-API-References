---
title: "Enum ResourceType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.ResourceType. Specifica il tipo di risorsa"
type: docs
weight: 1800
url: /it/net/aspose.tasks/resourcetype/
---
## ResourceType enumeration

Specifica il tipo di una risorsa.

```csharp
public enum ResourceType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Material | `0` | Indica il tipo di risorsa Materiale. |
| Work | `1` | Indica il tipo di risorsa Lavoro. |
| Cost | `2` | Indica il tipo di risorsa Costo. |

## Esempi

Mostra come lavorare con i tipi di risorsa.

```csharp
var project = new Project();

// aggiungi una risorsa di lavoro
var work = project.Resources.Add("Work resource");
work.Set(Rsc.Type, ResourceType.Work);

// aggiungi una risorsa materiale
var material = project.Resources.Add("Material resource");
material.Set(Rsc.Type, ResourceType.Material);
material.Set(Rsc.MaterialLabel, "kg");

// aggiungi una risorsa materiale
var cost = project.Resources.Add("Cost resource");
cost.Set(Rsc.Type, ResourceType.Cost);
cost.Set(Rsc.Cost, 59.99m);

// lavorare con le risorse: creare attività, assegnare risorse e così via...
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


