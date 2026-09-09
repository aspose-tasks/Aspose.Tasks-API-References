---
title: "PdfSaveOptions.Compliance"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PdfSaveOptions özelliği. Oluşturulan PDF belgesi için istenen uyumluluk seviyesini alır veya ayarlar. Varsayılan Pdf15'tir"
type: docs
weight: 20
url: /tr/net/aspose.tasks.saving/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Oluşturulan PDF belgesi için istenen uyumluluk seviyesini alır veya ayarlar. Varsayılan Pdf15'tir.

```csharp
public PdfCompliance Compliance { get; set; }
```

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

* enum [PdfCompliance](../../pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


