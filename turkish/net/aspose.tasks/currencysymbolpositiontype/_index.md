---
title: "Enum CurrencySymbolPositionType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.CurrencySymbolPositionType enum. Bir para birimi simgesinin konumunu belirtir"
type: docs
weight: 370
url: /tr/net/aspose.tasks/currencysymbolpositiontype/
---
## CurrencySymbolPositionType enumeration

Para birimi simgesinin konumunu belirtir.

```csharp
public enum CurrencySymbolPositionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `-1` | Tanımsız değerin, alanın orijinal proje dosyasında tanımlı olmadığı anlamına geldiğini gösterir. |
| Before | `0` | Para birimi simgesinden önce konum tipini gösterir. |
| After | `1` | Para birimi simgesinden sonra konum tipini gösterir. |
| BeforeWithSpace | `2` | Para birimi simgesiyle birlikte boşluk öncesi konum tipini gösterir. |
| AfterWithSpace | `3` | Para birimi simgesiyle birlikte boşluk sonrası konum tipini gösterir. |

## Açıklamalar

XML'e dışa aktarırken Tanımsız değerler sonuç XML'inden kaldırılacaktır.

## Örnekler

Para birimi simgesinin yerleşimini (CurrencySymbolPositionType.Before) nasıl belirteceğinizi gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
// para birimi simgesinin yerleşimini ayarla
// Önce, boşluk yok ($0).
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.Before);
// projeyle çalış...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


