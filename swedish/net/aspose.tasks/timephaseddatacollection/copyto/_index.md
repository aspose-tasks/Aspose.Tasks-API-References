---
title: TimephasedDataCollection.CopyTo
second_title: Aspose.Tasks för .NET API-referens
description: TimephasedDataCollection metod. Kopierar elementen iTimephasedDataCollection till enArray  börjar med en vissArray index.
type: docs
weight: 90
url: /sv/net/aspose.tasks/timephaseddatacollection/copyto/
---
## TimephasedDataCollection.CopyTo method

Kopierar elementen i[`TimephasedDataCollection`](../) till enArray , börjar med en vissArray index.

```csharp
public void CopyTo(TimephasedData[] array, int arrayIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| array | TimephasedData[] | Det endimensionellaArray det är destinationen för elementen som kopierats från[`TimephasedDataCollection`](../) . DenArray måste ha nollbaserad indexering. |
| arrayIndex | Int32 | Det nollbaserade indexet i*array* där kopieringen börjar. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *array* är inget. |
| ArgumentOutOfRangeException | *arrayIndex* är mindre än 0. |
| ArgumentException | Antalet element i källan[`TimephasedDataCollection`](../) är större än det tillgängliga utrymmet från*arrayIndex* till slutet av destinationen*array* . |

### Se även

* class [TimephasedData](../../timephaseddata/)
* class [TimephasedDataCollection](../)
* namnutrymme [Aspose.Tasks](../../timephaseddatacollection/)
* hopsättning [Aspose.Tasks](../../../)


