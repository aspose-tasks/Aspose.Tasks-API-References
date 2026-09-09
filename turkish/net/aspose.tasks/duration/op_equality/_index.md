---
title: "Duration.op_Equality"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Duration yöntemi. Bu örneğin belirtilen bir nesneye eşit olup olmadığını gösteren bir değer döndürür."
type: docs
weight: 140
url: /tr/net/aspose.tasks/duration/op_equality/
---
## Duration Equality operator

Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public static bool operator ==(Duration a, Duration b)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bir | Süre | İlk süre. |
| b | Süre | İkinci süre. |

### Dönüş Değeri

bu örneğin belirtilen bir nesneye eşit olup olmadığını gösteren bir değer

## Örnekler

Süre eşitliğini nasıl kontrol edeceğinizi gösterir.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// süre eşitliği, temel timespan'e karşı kontrol edilir.
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### Ayrıca Bakınız

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


