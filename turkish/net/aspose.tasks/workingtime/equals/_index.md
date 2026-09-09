---
title: "WorkingTime.Equals"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "WorkingTime yöntemi. Nesnelerin eşit olduğunu kontrol eder"
type: docs
weight: 40
url: /tr/net/aspose.tasks/workingtime/equals/
---
## WorkingTime.Equals method

Nesnelerin eşit olduğunu kontrol eder.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | Karşılaştırılacak ikinci nesne. |

### Dönüş Değeri

Nesneler eşitse true, aksi takdirde false.

## Örnekler

Çalışma zamanının eşitliğini nasıl kontrol edeceğini gösterir.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// Takvimlerin eşitliği, çalışma zamanının from ve to tarihleriyle karşılaştırılarak kontrol edilir.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### Ayrıca Bakınız

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


