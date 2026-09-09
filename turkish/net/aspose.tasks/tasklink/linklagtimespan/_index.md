---
title: "TaskLink.LinkLagTimeSpan"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskLink özelliği. LagFormat'a bağlı olarak gecikme süresini alır veya ayarlar"
type: docs
weight: 50
url: /tr/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

LagFormat'a bağlı olarak gecikme süresini alır veya ayarlar.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentException | LagFormat'ın TimeUnitType.Percent olduğu TaskLink'ler için değeri ayarlamaya çalışırken. |

## Açıklamalar

Bağlantı gecikmesi yüzde değeri olabilir (LagFormat TimeUnitType.Percent'tir). Bu durumda süre, PredTask'ın süresinin yüzde olarak hesaplanır. Aksi takdirde yöntem, TaskLink'in gecikmesini temsil eden TimeSpan değerini döndürür.

### Ayrıca Bakınız

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


