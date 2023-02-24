---
title: TimephasedData.CreateWorkTimephased
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: TimephasedData metodo. Crea e inizializza una nuova istanza diTimephasedData classe per dati cronologici basati sul lavoro.
type: docs
weight: 40
url: /it/net/aspose.tasks/timephaseddata/createworktimephased/
---
## TimephasedData.CreateWorkTimephased method

Crea e inizializza una nuova istanza di[`TimephasedData`](../) classe per dati cronologici basati sul lavoro.

```csharp
public static TimephasedData CreateWorkTimephased(int uid, DateTime start, DateTime finish, 
    TimeSpan value, TimeUnitType timeUnit, TimephasedDataType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | Int32 | UID dell'attività. |
| start | DateTime | data-ora di inizio. |
| finish | DateTime | Fine data-ora. |
| value | TimeSpan | Valore dell'intervallo di tempo. |
| timeUnit | TimeUnitType | Tipo di unità di tempo. |
| type | TimephasedDataType | Tipo di dati rapportato alla scala cronologica. |

### Valore di ritorno

Un'istanza di[`TimephasedData`](../) classe per dati cronologici basati sul lavoro.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Se è stato specificato un valore di lavoro negativo. |

### Guarda anche

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* spazio dei nomi [Aspose.Tasks](../../timephaseddata/)
* assemblea [Aspose.Tasks](../../../)


