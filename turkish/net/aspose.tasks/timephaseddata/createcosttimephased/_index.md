---
title: TimephasedData.CreateCostTimephased
second_title: Aspose.Tasks for .NET API Referansı
description: TimephasedData yöntem. Yeni bir örnek oluşturur ve başlatır.TimephasedData maliyete dayalı zaman aşamalı veriler için sınıf.
type: docs
weight: 20
url: /tr/net/aspose.tasks/timephaseddata/createcosttimephased/
---
## TimephasedData.CreateCostTimephased method

Yeni bir örnek oluşturur ve başlatır.[`TimephasedData`](../) maliyete dayalı zaman aşamalı veriler için sınıf.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimeUnitType timeUnit, TimephasedDataType type)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| uid | Int32 | Görevin UID'si. |
| start | DateTime | tarih-zamanı başlat. |
| finish | DateTime | Tarih-zamanı bitir. |
| value | Double | Maliyet değeri. |
| timeUnit | TimeUnitType | Zaman birimi türü. |
| type | TimephasedDataType | Zaman aşamalı veri türü. |

### Geri dönüş değeri

bir örneği[`TimephasedData`](../) maliyete dayalı zaman aşamalı veriler için sınıf.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentException | Negatif maliyet değeri belirtilmişse. |

### Ayrıca bakınız

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* ad alanı [Aspose.Tasks](../../timephaseddata/)
* toplantı [Aspose.Tasks](../../../)


