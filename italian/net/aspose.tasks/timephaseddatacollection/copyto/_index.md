---
title: TimephasedDataCollection.CopyTo
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: TimephasedDataCollection metodo. Copia gli elementi del fileTimephasedDataCollection adArray  partendo da un particolareArray indice.
type: docs
weight: 90
url: /it/net/aspose.tasks/timephaseddatacollection/copyto/
---
## TimephasedDataCollection.CopyTo method

Copia gli elementi del file[`TimephasedDataCollection`](../) adArray , partendo da un particolareArray indice.

```csharp
public void CopyTo(TimephasedData[] array, int arrayIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| array | TimephasedData[] | L'unidimensionaleArray questa è la destinazione degli elementi copiati da[`TimephasedDataCollection`](../) . IlArray deve avere un'indicizzazione in base zero. |
| arrayIndex | Int32 | L'indice in base zero in*array* in cui inizia la copiatura. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *array* è zero. |
| ArgumentOutOfRangeException | *arrayIndex* è minore di 0. |
| ArgumentException | Il numero di elementi nell'origine[`TimephasedDataCollection`](../) è maggiore dello spazio disponibile da*arrayIndex* alla fine della destinazione*array* . |

### Guarda anche

* class [TimephasedData](../../timephaseddata/)
* class [TimephasedDataCollection](../)
* spazio dei nomi [Aspose.Tasks](../../timephaseddatacollection/)
* assemblea [Aspose.Tasks](../../../)


