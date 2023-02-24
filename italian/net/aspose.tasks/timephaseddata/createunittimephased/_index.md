---
title: TimephasedData.CreateUnitTimephased
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: TimephasedData metodo. Crea e inizializza una nuova istanza diTimephasedData classe per i dati in scala temporale basati su unità di unassegnazione di una risorsa materiale.
type: docs
weight: 30
url: /it/net/aspose.tasks/timephaseddata/createunittimephased/
---
## TimephasedData.CreateUnitTimephased method

Crea e inizializza una nuova istanza di[`TimephasedData`](../) classe per i dati in scala temporale basati su unità di un'assegnazione di una risorsa materiale.

```csharp
public static TimephasedData CreateUnitTimephased(int uid, DateTime start, DateTime finish, 
    double units, TimephasedDataType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | Int32 | UID dell'attività. |
| start | DateTime | Data e ora di inizio. |
| finish | DateTime | Fine data-ora. |
| units | Double | Numero di unità. |
| type | TimephasedDataType | Tipo di dati rapportato alla scala cronologica. |

### Valore di ritorno

Un'istanza di[`TimephasedData`](../) classe per dati temporizzati basati sui costi.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Se è stato specificato un numero di unità negativo. |

### Guarda anche

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* spazio dei nomi [Aspose.Tasks](../../timephaseddata/)
* assemblea [Aspose.Tasks](../../../)


