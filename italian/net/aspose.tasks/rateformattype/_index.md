---
title: "Enum RateFormatType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.RateFormatType. Specifica le unità usate da Microsoft Project per visualizzare una tariffa."
type: docs
weight: 1640
url: /it/net/aspose.tasks/rateformattype/
---
## RateFormatType enumeration

Specifica le unità utilizzate da Microsoft Project per visualizzare un tasso.

```csharp
public enum RateFormatType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `-1` | Il valore non era definito nel file di progetto originale. |
| Minute | `0` | Minuto ("min") |
| Hour | `1` | Ora ("hr") |
| Day | `2` | Giorno ("day") |
| Week | `3` | Settimana ("wk") |
| Month | `4` | Mese ("mo") |
| Year | `5` | Anno ("yr") |
| MaterialResourceRate | `6` | Tariffa risorsa materiale (vuoto) |

## Osservazioni

Durante l'esportazione in XML i valori Undefined verranno eliminati dall'XML risultante.

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.StandardRateFormat.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


