---
title: TimephasedDataCollection.SelectBetweenStartAndFinish
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: TimephasedDataCollection metodo. Seleziona tutte le fasce orarie trastartTime EfinishTime . Ha complessità Olog n nel caso medio.
type: docs
weight: 120
url: /it/net/aspose.tasks/timephaseddatacollection/selectbetweenstartandfinish/
---
## TimephasedDataCollection.SelectBetweenStartAndFinish method

Seleziona tutte le fasce orarie tra*startTime* E*finishTime* . Ha complessità O(log n) nel caso medio.

```csharp
public IList<TimephasedData> SelectBetweenStartAndFinish(TimephasedDataType timephasedDataType, 
    DateTime startTime, DateTime finishTime)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| timephasedDataType | TimephasedDataType | Tipo di fasce orarie da selezionare. |
| startTime | DateTime | Inizio dell'intervallo. |
| finishTime | DateTime | Fine dell'intervallo. |

### Valore di ritorno

Restituisce una nuova istanza di elenco di[`TimephasedDataCollection`](../) dati ordinati per proprietà Inizio.

### Guarda anche

* class [TimephasedData](../../timephaseddata/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedDataCollection](../)
* spazio dei nomi [Aspose.Tasks](../../timephaseddatacollection/)
* assemblea [Aspose.Tasks](../../../)


