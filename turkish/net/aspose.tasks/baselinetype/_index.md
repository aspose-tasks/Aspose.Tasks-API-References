---
title: "Enum BaselineType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.BaselineType enum. Varyans değerlerini hesaplamak için kullanılan temel çizgi tipini belirtir."
type: docs
weight: 130
url: /tr/net/aspose.tasks/baselinetype/
---
## BaselineType enumeration

Varyans değerlerini hesaplamak için kullanılan temel çizgi tipini belirtir.

```csharp
public enum BaselineType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `-1` | Alanının orijinal proje dosyasında tanımlanmadığını gösterir. |
| Baseline | `0` | Temel çizgi tipini gösterir. |
| Baseline1 | `1` | Baseline1 tipini gösterir. |
| Baseline2 | `2` | Baseline2 tipini gösterir. |
| Baseline3 | `3` | Baseline3 tipini gösterir. |
| Baseline4 | `4` | Baseline4 tipini gösterir. |
| Baseline5 | `5` | Baseline5 tipini gösterir. |
| Baseline6 | `6` | Baseline6 tipini gösterir. |
| Baseline7 | `7` | Baseline7 tipini gösterir. |
| Baseline8 | `8` | Baseline8 tipini gösterir. |
| Baseline9 | `9` | Baseline9 tipini gösterir. |
| Baseline10 | `10` | Baseline10 tipini gösterir. |

## Açıklamalar

XML'e dışa aktarırken Tanımsız değerler sonuç XML'inden kaldırılacaktır.

## Örnekler

Proje için temel çizgiyi (BaselineType.Baseline) nasıl ayarlayacağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
// Tüm proje için belirtilen temel çizgiye temel çizgi alanlarını kaydedin.
project.SetBaseline(BaselineType.Baseline);
// projenin temel çizgileriyle çalışın...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


