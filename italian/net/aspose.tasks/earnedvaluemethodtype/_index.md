---
title: "Enum EarnedValueMethodType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.EarnedValueMethodType. Specifica il metodo utilizzato per calcolare il valore guadagnato"
type: docs
weight: 480
url: /it/net/aspose.tasks/earnedvaluemethodtype/
---
## EarnedValueMethodType enumeration

Specifica il metodo utilizzato per calcolare il valore guadagnato.

```csharp
public enum EarnedValueMethodType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `-1` | Il campo non era definito nel file di progetto originale. |
| PercentComplete | `0` | Percentuale completata |
| PhysicalPercentComplete | `1` | Percentuale fisica completata |

## Osservazioni

Durante l'esportazione in XML i valori Undefined verranno eliminati dall'XML risultante.

## Esempi

Mostra come specificare il metodo utilizzato per calcolare il valore guadagnato (EarnedValueMethodType.PercentComplete).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// impostare il tipo di metodo del valore guadagnato su 'PercentComplete'
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
// lavorare con il progetto...
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


