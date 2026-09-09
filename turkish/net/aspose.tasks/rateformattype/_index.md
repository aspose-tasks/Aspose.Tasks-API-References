---
title: "Enum RateFormatType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.RateFormatType enum. Microsoft Project'in bir oranı görüntülemek için kullandığı birimleri belirtir."
type: docs
weight: 1640
url: /tr/net/aspose.tasks/rateformattype/
---
## RateFormatType enumeration

Microsoft Project'in bir oranı görüntülemek için kullandığı birimleri belirtir.

```csharp
public enum RateFormatType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `-1` | Değer, orijinal proje dosyasında tanımlanmamıştı. |
| Minute | `0` | Dakika ("min") |
| Hour | `1` | Saat ("hr") |
| Day | `2` | Gün ("day") |
| Week | `3` | Hafta ("wk") |
| Month | `4` | Ay ("mo") |
| Year | `5` | Yıl ("yr") |
| MaterialResourceRate | `6` | Malzeme kaynak oranı (boş) |

## Açıklamalar

XML'e dışa aktarırken Tanımsız değerler sonuç XML'inden kaldırılacaktır.

## Örnekler

Rsc.StandardRateFormat özelliğini okuma/yazma işleminin nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


