---
title: "Enum PdfTextCompression"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.PdfTextCompression enum. PDF dosyasındaki görüntüler dışındaki tüm içeriğe uygulanan sıkıştırma türünü belirtir."
type: docs
weight: 2140
url: /tr/net/aspose.tasks.saving/pdftextcompression/
---
## PdfTextCompression enumeration

PDF dosyasındaki görüntüler dışındaki tüm içeriğe uygulanan sıkıştırma türünü belirtir.

```csharp
public enum PdfTextCompression
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Sıkıştırma yok. |
| Flate | `1` | Flate sıkıştırması. |

## Örnekler

Görüntüler dışındaki tüm içerik akışları için kullanılacak bir sıkıştırma türünün nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// görüntüler dışındaki tüm içerik akışları için kullanılacak sıkıştırma türünü ayarla
options.TextCompression = PdfTextCompression.Flate;

// ek özellikleri ayarla
// belgenin kaydedileceği <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> ayarla.
options.PresentationFormat = PresentationFormat.GanttChart;

// oluşturulan PDF belgesi için istenen uyumluluk seviyesini ayarla
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithTextCompression_out.pdf", options);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


