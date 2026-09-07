---
title: "Duration.ParseTimeSpan"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Duration. Analizza la stringa di durata nel formato PTHMS"
type: docs
weight: 130
url: /it/net/aspose.tasks/duration/parsetimespan/
---
## Duration.ParseTimeSpan method

Analizza la stringa di durata nel formato "PT--H--M--S--".

```csharp
public static TimeSpan ParseTimeSpan(string value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | Stringa | la stringa specificata da analizzare. |

### Valore di ritorno

restituisce l'istanza analizzata della struttura [`TimeSpan`](../timespan/).

## Esempi

Mostra come convertire una stringa in un intervallo di tempo.

```csharp
var timeSpan = Duration.ParseTimeSpan("PT1H10M30S");
Console.WriteLine("The parsed time span: " + timeSpan);
```

### Vedi anche

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


