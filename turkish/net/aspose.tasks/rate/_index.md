---
title: "Rate sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Rate sınıfı. Bir zaman diliminin tanımını ve bu dönemde bir kaynak için geçerli olan oranları temsil eder."
type: docs
weight: 1610
url: /tr/net/aspose.tasks/rate/
---
## Rate class

Bir zaman diliminin tanımını ve bu süre içinde bir kaynak için geçerli olan oranları temsil eder.

```csharp
public class Rate
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CostPerUse](../../aspose.tasks/rate/costperuse/) { get; set; } | Bir kaynağın kullanım başına maliyetini alır veya ayarlar. Bu değer, kaynak için bir oran tablosu mevcutsa geçerli tarihten alınır. |
| [OvertimeRate](../../aspose.tasks/rate/overtimerate/) { get; set; } | Bir kaynak için saat başına fazla mesai oranını alır veya ayarlar. |
| [OvertimeRateFormat](../../aspose.tasks/rate/overtimerateformat/) { get; set; } | Microsoft Project'in fazla mesai oranını görüntülemek için kullandığı birimleri alır veya ayarlar. |
| [RatesFrom](../../aspose.tasks/rate/ratesfrom/) { get; set; } | Bir oranının yürürlüğe girdiği tarihi alır veya ayarlar. |
| [RatesTo](../../aspose.tasks/rate/ratesto/) { get; set; } | Bir oranının geçerli olduğu son tarihi alır veya ayarlar. |
| [RateTable](../../aspose.tasks/rate/ratetable/) { get; set; } | Bir kaynak için oran tablosunun benzersiz tanımlayıcısını alır veya ayarlar. |
| [StandardRate](../../aspose.tasks/rate/standardrate/) { get; set; } | Bir kaynak için saat başına standart oranı alır veya ayarlar. |
| [StandardRateFormat](../../aspose.tasks/rate/standardrateformat/) { get; set; } | Microsoft Project'in standart oranı görüntülemek için kullandığı birimleri alır veya ayarlar. |

## Örnekler

Kaynak oranlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RateTable = RateType.A;
rate1.RatesFrom = new DateTime(2019, 1, 1, 8, 0, 0);
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;
rate1.OvertimeRate = 10m;
rate1.OvertimeRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0));
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;
rate2.CostPerUse = 2m;

// projeyle çalış...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


