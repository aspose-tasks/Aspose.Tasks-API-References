---
title: TimephasedDataCollection.CopyTo
second_title: Aspose.Tasks for .NET API Referansı
description: TimephasedDataCollection yöntem. öğesinin öğelerini kopyalar.TimephasedDataCollection birArray  belirli bir noktadan başlayarakArray dizin.
type: docs
weight: 90
url: /tr/net/aspose.tasks/timephaseddatacollection/copyto/
---
## TimephasedDataCollection.CopyTo method

öğesinin öğelerini kopyalar.[`TimephasedDataCollection`](../) birArray , belirli bir noktadan başlayarakArray dizin.

```csharp
public void CopyTo(TimephasedData[] array, int arrayIndex)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| array | TimephasedData[] | tek boyutluArray bu, kopyalanan öğelerin hedefidir[`TimephasedDataCollection`](../) . Array sıfır tabanlı indekslemeye sahip olmalıdır. |
| arrayIndex | Int32 | sıfır tabanlı dizin*array* kopyalamanın başladığı yer. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *array* boş. |
| ArgumentOutOfRangeException | *arrayIndex* 0'dan küçüktür. |
| ArgumentException | Kaynaktaki öğelerin sayısı[`TimephasedDataCollection`](../) mevcut alandan daha büyük*arrayIndex* hedefin sonuna*array* . |

### Ayrıca bakınız

* class [TimephasedData](../../timephaseddata/)
* class [TimephasedDataCollection](../)
* ad alanı [Aspose.Tasks](../../timephaseddatacollection/)
* toplantı [Aspose.Tasks](../../../)


