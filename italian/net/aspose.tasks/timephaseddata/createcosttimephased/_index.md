---
title: TimephasedData.CreateCostTimephased
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: TimephasedData metodo. Crea e inizializza una nuova istanza diTimephasedData classe per dati in scala temporale basati sui costi.
type: docs
weight: 20
url: /it/net/aspose.tasks/timephaseddata/createcosttimephased/
---
## TimephasedData.CreateCostTimephased method

Crea e inizializza una nuova istanza di[`TimephasedData`](../) classe per dati in scala temporale basati sui costi.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimeUnitType timeUnit, TimephasedDataType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | Int32 | UID dell'attività. |
| start | DateTime | data-ora di inizio. |
| finish | DateTime | Fine data-ora. |
| value | Double | Valore di costo. |
| timeUnit | TimeUnitType | Tipo di unità di tempo. |
| type | TimephasedDataType | Tipo di dati rapportato alla scala cronologica. |

### Valore di ritorno

Un'istanza di[`TimephasedData`](../) classe per dati temporizzati basati sui costi.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Se è stato specificato un valore di costo negativo. |

### Guarda anche

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* spazio dei nomi [Aspose.Tasks](../../timephaseddata/)
* assemblea [Aspose.Tasks](../../../)


