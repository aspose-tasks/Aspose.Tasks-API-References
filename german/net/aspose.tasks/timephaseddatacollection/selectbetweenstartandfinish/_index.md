---
title: TimephasedDataCollection.SelectBetweenStartAndFinish
second_title: Aspose.Tasks für .NET-API-Referenz
description: TimephasedDataCollection methode. Wählt alle Zeitphasen dazwischen ausstartTime UndfinishTime . Hat Olog n Komplexität im Durchschnittsfall.
type: docs
weight: 120
url: /de/net/aspose.tasks/timephaseddatacollection/selectbetweenstartandfinish/
---
## TimephasedDataCollection.SelectBetweenStartAndFinish method

Wählt alle Zeitphasen dazwischen aus*startTime* Und*finishTime* . Hat O(log n) Komplexität im Durchschnittsfall.

```csharp
public IList<TimephasedData> SelectBetweenStartAndFinish(TimephasedDataType timephasedDataType, 
    DateTime startTime, DateTime finishTime)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| timephasedDataType | TimephasedDataType | Art der auszuwählenden Zeitphasen. |
| startTime | DateTime | Beginn des Intervalls. |
| finishTime | DateTime | Ende des Intervalls. |

### Rückgabewert

Gibt eine neue Listeninstanz von zurück[`TimephasedDataCollection`](../) Daten sortiert nach Start-Eigenschaft.

### Siehe auch

* class [TimephasedData](../../timephaseddata/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedDataCollection](../)
* namensraum [Aspose.Tasks](../../timephaseddatacollection/)
* Montage [Aspose.Tasks](../../../)


