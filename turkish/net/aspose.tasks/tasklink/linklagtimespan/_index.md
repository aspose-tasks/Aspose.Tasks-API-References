---
title: TaskLink.LinkLagTimeSpan
second_title: Aspose.Tasks for .NET API Referansı
description: TaskLink mülk. LagFormata bağlı olarak gecikme süresini alır veya ayarlar.
type: docs
weight: 50
url: /tr/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

LagFormat'a bağlı olarak gecikme süresini alır veya ayarlar.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentException | LagFormat'ın TimeUnitType.Percent olduğu TaskLinks değerini ayarlamaya çalışırken. |

### Notlar

Bağlantı gecikmesi bir yüzde değeri olabilir (LagFormat, TimeUnitType.Percent). Bu durumda süre, PredTask süresinin yüzdesi olarak hesaplanır. Aksi takdirde, yöntem, TaskLink'in gecikmesini temsil eden TimeSpan değerini döndürür.

### Ayrıca bakınız

* class [TaskLink](../)
* ad alanı [Aspose.Tasks](../../tasklink/)
* toplantı [Aspose.Tasks](../../../)


