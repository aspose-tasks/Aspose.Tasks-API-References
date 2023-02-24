---
title: TimephasedDataCollection.SelectBetweenStartAndFinish
second_title: Aspose.Tasks för .NET API-referens
description: TimephasedDataCollection metod. Väljer alla tidsfaser mellanstartTime ochfinishTime . Har Olog n komplexitet i genomsnittligt fall.
type: docs
weight: 120
url: /sv/net/aspose.tasks/timephaseddatacollection/selectbetweenstartandfinish/
---
## TimephasedDataCollection.SelectBetweenStartAndFinish method

Väljer alla tidsfaser mellan*startTime* och*finishTime* . Har O(log n) komplexitet i genomsnittligt fall.

```csharp
public IList<TimephasedData> SelectBetweenStartAndFinish(TimephasedDataType timephasedDataType, 
    DateTime startTime, DateTime finishTime)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| timephasedDataType | TimephasedDataType | Typ av tidsfaser att välja. |
| startTime | DateTime | Intervalls start. |
| finishTime | DateTime | Intervalls avslutning. |

### Returvärde

Returnerar ny listinstans av[`TimephasedDataCollection`](../) data sorterad av Start-egenskapen.

### Se även

* class [TimephasedData](../../timephaseddata/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedDataCollection](../)
* namnutrymme [Aspose.Tasks](../../timephaseddatacollection/)
* hopsättning [Aspose.Tasks](../../../)


