---
title: "PdfSaveOptions.TextCompression"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PdfSaveOptions. Mendapatkan atau mengatur jenis kompresi yang akan digunakan untuk semua aliran konten kecuali gambar. Defaultnya adalah Flate"
type: docs
weight: 100
url: /id/net/aspose.tasks.saving/pdfsaveoptions/textcompression/
---
## PdfSaveOptions.TextCompression property

Mendapatkan atau mengatur jenis kompresi yang akan digunakan untuk semua aliran konten kecuali gambar. Defaultnya adalah Flate.

```csharp
public PdfTextCompression TextCompression { get; set; }
```

## Contoh

Menampilkan cara mengatur jenis kompresi yang akan digunakan untuk semua aliran konten kecuali gambar.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// atur jenis kompresi yang akan digunakan untuk semua aliran konten kecuali gambar
options.TextCompression = PdfTextCompression.Flate;

// sesuaikan properti tambahan
// atur <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> di mana dokumen akan disimpan.
options.PresentationFormat = PresentationFormat.GanttChart;

// atur tingkat kepatuhan yang diinginkan untuk dokumen PDF yang dihasilkan
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithTextCompression_out.pdf", options);
```

### Lihat Juga

* enum [PdfTextCompression](../../pdftextcompression/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


