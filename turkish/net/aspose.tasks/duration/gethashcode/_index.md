---
title: "Duration.GetHashCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Duration yöntemi. Bu nesne için bir karma kod değeri döndürür."
type: docs
weight: 90
url: /tr/net/aspose.tasks/duration/gethashcode/
---
## Duration.GetHashCode method

Bu nesne için bir karma kod değeri döndürür.

```csharp
public override int GetHashCode()
```

### Dönüş Değeri

Bu süre örneği için bir karma kod değeri döndürür.

## Örnekler

Bir sürenin karma kodunu nasıl alacağınızı gösterir.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// Bir takvimin karma kodu, zaman birimi türüne ve sürenin başlangıç değerine dayanır.
// bu yüzden sonraki karma kodlar eşittir.
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 2 Hash Code: {0}", duration2.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration2.GetHashCode()));

// ancak süre 1 ve 3'ün karma kodları eşit değildir.
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 3 Hash Code: {0}", duration3.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration3.GetHashCode()));
```

### Ayrıca Bakınız

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


