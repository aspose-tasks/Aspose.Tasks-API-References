---
title: "PdfSaveOptions.EncryptionDetails"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PdfSaveOptions. Mendapatkan atau mengatur detail enkripsi. Jika tidak diatur maka tidak akan ada enkripsi yang dilakukan"
type: docs
weight: 40
url: /id/net/aspose.tasks.saving/pdfsaveoptions/encryptiondetails/
---
## PdfSaveOptions.EncryptionDetails property

Mendapatkan atau mengatur detail enkripsi. Jika tidak diatur, maka tidak akan ada enkripsi yang dilakukan.

```csharp
public PdfEncryptionDetails EncryptionDetails { get; set; }
```

## Contoh

Menampilkan cara mengatur detail enkripsi dokumen PDF. Jika tidak diatur, maka tidak akan ada enkripsi yang dilakukan.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var encryptionDetails = new PdfEncryptionDetails("userPassword", "ownerPassword", PdfEncryptionAlgorithm.RC4_128);

var options = new PdfSaveOptions();

// atur detail enkripsi dokumen PDF
options.EncryptionDetails = encryptionDetails;

// sesuaikan properti tambahan
// atur <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> di mana dokumen akan disimpan.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithEncryptionDetails_out.pdf", options);
```

### Lihat Juga

* class [PdfEncryptionDetails](../../pdfencryptiondetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


