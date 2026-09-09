---
title: "Enum PdfCompliance"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.PdfCompliance enum. PDF uyumluluk seviyesini çıktı dosyasına belirtir."
type: docs
weight: 2070
url: /tr/net/aspose.tasks.saving/pdfcompliance/
---
## PdfCompliance enumeration

Çıktı dosyası için PDF uyumluluk seviyesini belirtir.

```csharp
public enum PdfCompliance
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Pdf15 | `0` | PDF/15 uyumluluk seviyesi. |
| PdfA1a | `1` | PDF/A-1a uyumluluk seviyesi. |
| PdfA1b | `2` | PDF/A-1b uyumluluk seviyesi. |

## Örnekler

Oluşturulan PDF belgesi için istenen uyumluluk seviyesinin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// oluşturulan PDF belgesi için istenen uyumluluk seviyesini ayarla
// varsayılan <see cref=\"PdfCompliance.Pdf15\"/> tipidir.
options.Compliance = PdfCompliance.PdfA1b;

// ek özellikleri ayarla
// belgenin kaydedileceği <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> ayarla.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithPdfCompliance_out.pdf", options);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


