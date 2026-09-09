---
title: "Duration.ParseTimeSpan"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Duration yöntemi. PTHMS formatındaki süre dizesini ayrıştırır."
type: docs
weight: 130
url: /tr/net/aspose.tasks/duration/parsetimespan/
---
## Duration.ParseTimeSpan method

\"PT--H--M--S--\" biçimindeki süre dizesini ayrıştırır.

```csharp
public static TimeSpan ParseTimeSpan(string value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | Dize | ayrıştırılacak belirtilen dize. |

### Dönüş Değeri

parçalanmış bir [`TimeSpan`](../timespan/) yapısının örneğini döndürür.

## Örnekler

Bir dizeyi zaman aralığına nasıl dönüştüreceğinizi gösterir.

```csharp
var timeSpan = Duration.ParseTimeSpan("PT1H10M30S");
Console.WriteLine("The parsed time span: " + timeSpan);
```

### Ayrıca Bakınız

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


