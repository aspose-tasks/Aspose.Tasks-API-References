---
title: "PdfSaveOptions.TextCompression"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PdfSaveOptions özelliği. Görseller dışındaki tüm içerik akışları için kullanılacak bir sıkıştırma türünü alır veya ayarlar. Varsayılan Flate'tir"
type: docs
weight: 100
url: /tr/net/aspose.tasks.saving/pdfsaveoptions/textcompression/
---
## PdfSaveOptions.TextCompression property

Görseller dışındaki tüm içerik akışları için kullanılacak sıkıştırma türünü alır veya ayarlar. Varsayılan Flate'tir.

```csharp
public PdfTextCompression TextCompression { get; set; }
```

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

* enum [PdfTextCompression](../../pdftextcompression/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


