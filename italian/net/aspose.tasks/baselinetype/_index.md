---
title: "Enum BaselineType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.BaselineType. Specifica il tipo di baseline utilizzato per calcolare i valori di Varianza."
type: docs
weight: 130
url: /it/net/aspose.tasks/baselinetype/
---
## BaselineType enumeration

Specifica il tipo di baseline utilizzato per calcolare i valori di varianza.

```csharp
public enum BaselineType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `-1` | Indica che il campo non è stato definito nel file di progetto originale. |
| Baseline | `0` | Indica il tipo di Baseline. |
| Baseline1 | `1` | Indica il tipo di Baseline1. |
| Baseline2 | `2` | Indica il tipo di Baseline2. |
| Baseline3 | `3` | Indica il tipo di Baseline3. |
| Baseline4 | `4` | Indica il tipo di Baseline4. |
| Baseline5 | `5` | Indica il tipo di Baseline5. |
| Baseline6 | `6` | Indica il tipo di Baseline6. |
| Baseline7 | `7` | Indica il tipo di Baseline7. |
| Baseline8 | `8` | Indica il tipo di Baseline8. |
| Baseline9 | `9` | Indica il tipo di Baseline9. |
| Baseline10 | `10` | Indica il tipo di Baseline10. |

## Osservazioni

Durante l'esportazione in XML i valori Undefined verranno eliminati dall'XML risultante.

## Esempi

Mostra come impostare la baseline per il progetto (BaselineType.Baseline).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// Salva i campi della baseline nella baseline specificata per l'intero progetto.
project.SetBaseline(BaselineType.Baseline);
// Lavora con le baseline del progetto...
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


