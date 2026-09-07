---
title: "PdfSaveOptions.DigitalSignatureDetails"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PdfSaveOptions. Mendapatkan atau mengatur detail tanda tangan digital. Jika tidak diatur maka tidak akan ada penandatanganan yang dilakukan"
type: docs
weight: 30
url: /id/net/aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/
---
## PdfSaveOptions.DigitalSignatureDetails property

Mendapatkan atau mengatur detail tanda tangan digital. Jika tidak diatur, maka tidak akan ada penandatanganan yang dilakukan.

```csharp
public PdfDigitalSignatureDetails DigitalSignatureDetails { get; set; }
```

## Contoh

Menampilkan cara mengatur detail tanda tangan digital. Jika tidak diatur, maka tidak akan ada penandatanganan yang dilakukan.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
var certificate = new X509Certificate2();

// atur detail tanda tangan digital. Jika tidak diatur, maka tidak akan ada penandatanganan yang dilakukan.
options.DigitalSignatureDetails = new PdfDigitalSignatureDetails(
    certificate,
    "reason",
    "location",
    new DateTime(2019, 1, 1),
    PdfDigitalSignatureHashAlgorithm.Sha1);

// sesuaikan properti tambahan
// atur <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> di mana dokumen akan disimpan.
options.PresentationFormat = PresentationFormat.GanttChart;

// atur tingkat kepatuhan yang diinginkan untuk dokumen PDF yang dihasilkan
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithDigitalSignatureDetails_out.pdf", options);
```

### Lihat Juga

* class [PdfDigitalSignatureDetails](../../pdfdigitalsignaturedetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


