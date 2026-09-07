---
title: "Enum PdfTextCompression"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Saving.PdfTextCompression. Menentukan jenis kompresi yang diterapkan pada semua konten dalam file PDF kecuali gambar."
type: docs
weight: 2140
url: /id/net/aspose.tasks.saving/pdftextcompression/
---
## PdfTextCompression enumeration

Menentukan jenis kompresi yang diterapkan pada semua konten dalam file PDF kecuali gambar.

```csharp
public enum PdfTextCompression
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| None | `0` | Tanpa kompresi. |
| Flate | `1` | Kompressi Flate. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


