---
title: "PdfSaveOptions.DigitalSignatureDetails"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PdfSaveOptions özelliği. Dijital imza ayrıntılarını alır veya ayarlar. Ayarlanmamışsa imzalama yapılmaz"
type: docs
weight: 30
url: /tr/net/aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/
---
## PdfSaveOptions.DigitalSignatureDetails property

Dijital imza ayrıntılarını alır veya ayarlar. Ayarlanmamışsa, imzalama yapılmaz.

```csharp
public PdfDigitalSignatureDetails DigitalSignatureDetails { get; set; }
```

## Örnekler

Dijital imza ayrıntılarını nasıl ayarlayacağınızı gösterir. Ayarlanmamışsa imzalama yapılmaz.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
var certificate = new X509Certificate2();

// dijital imza ayrıntılarını ayarlayın. Ayarlanmamışsa imzalama yapılmaz.
options.DigitalSignatureDetails = new PdfDigitalSignatureDetails(
    certificate,
    "reason",
    "location",
    new DateTime(2019, 1, 1),
    PdfDigitalSignatureHashAlgorithm.Sha1);

// ek özellikleri ayarla
// belgenin kaydedileceği <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> ayarla.
options.PresentationFormat = PresentationFormat.GanttChart;

// oluşturulan PDF belgesi için istenen uyumluluk seviyesini ayarla
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithDigitalSignatureDetails_out.pdf", options);
```

### Ayrıca Bakınız

* class [PdfDigitalSignatureDetails](../../pdfdigitalsignaturedetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


