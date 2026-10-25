---
title: "PdfSaveOptions.EncryptionDetails"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PdfSaveOptions özelliği. Şifreleme ayrıntılarını alır veya ayarlar. Ayarlanmamışsa şifreleme yapılmaz"
type: docs
weight: 40
url: /tr/net/aspose.tasks.saving/pdfsaveoptions/encryptiondetails/
---
## PdfSaveOptions.EncryptionDetails property

Şifreleme ayrıntılarını alır veya ayarlar. Ayarlanmamışsa, şifreleme yapılmaz.

```csharp
public PdfEncryptionDetails EncryptionDetails { get; set; }
```

## Örnekler

PDF belgesinin şifreleme ayrıntılarını nasıl ayarlayacağınızı gösterir. Ayarlanmamışsa şifreleme yapılmaz.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var encryptionDetails = new PdfEncryptionDetails("userPassword", "ownerPassword", PdfEncryptionAlgorithm.RC4_128);

var options = new PdfSaveOptions();

// PDF belgesinin şifreleme ayrıntılarını ayarlayın
options.EncryptionDetails = encryptionDetails;

// ek özellikleri ayarla
// belgenin kaydedileceği <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> ayarla.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithEncryptionDetails_out.pdf", options);
```

### Ayrıca Bakınız

* class [PdfEncryptionDetails](../../pdfencryptiondetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


