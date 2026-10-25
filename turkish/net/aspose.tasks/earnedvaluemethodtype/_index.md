---
title: "Enum EarnedValueMethodType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.EarnedValueMethodType enum. Kazanılmış değerin hesaplanmasında kullanılan yöntemi belirtir"
type: docs
weight: 480
url: /tr/net/aspose.tasks/earnedvaluemethodtype/
---
## EarnedValueMethodType enumeration

Kazanılan değerin hesaplanmasında kullanılan yöntemi belirtir.

```csharp
public enum EarnedValueMethodType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `-1` | Alan, orijinal proje dosyasında tanımlanmamıştı. |
| PercentComplete | `0` | Tamamlanma yüzdesi |
| PhysicalPercentComplete | `1` | Fiziksel tamamlanma yüzdesi |

## Açıklamalar

XML'e dışa aktarırken Tanımsız değerler sonuç XML'inden kaldırılacaktır.

## Örnekler

Kazanılmış değerin hesaplanmasında kullanılan yöntemin (EarnedValueMethodType.PercentComplete) nasıl belirtileceğini gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
// kazanılmış değer yöntemi tipini 'PercentComplete' olarak ayarla
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
// projeyle çalış...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


