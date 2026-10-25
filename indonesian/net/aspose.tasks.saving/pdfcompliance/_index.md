---
title: "Enum PdfCompliance"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Saving.PdfCompliance. Menentukan tingkat kepatuhan PDF untuk file keluaran."
type: docs
weight: 2070
url: /id/net/aspose.tasks.saving/pdfcompliance/
---
## PdfCompliance enumeration

Menentukan tingkat kepatuhan PDF untuk file output.

```csharp
public enum PdfCompliance
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Pdf15 | `0` | Tingkat kepatuhan PDF/15. |
| PdfA1a | `1` | Tingkat kepatuhan PDF/A-1a. |
| PdfA1b | `2` | Tingkat kepatuhan PDF/A-1b. |

## Contoh

Menampilkan cara mengatur tingkat kepatuhan yang diinginkan untuk dokumen PDF yang dihasilkan.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// atur tingkat kepatuhan yang diinginkan untuk dokumen PDF yang dihasilkan
// default adalah tipe <see cref=\"PdfCompliance.Pdf15\"/>
options.Compliance = PdfCompliance.PdfA1b;

// sesuaikan properti tambahan
// atur <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> di mana dokumen akan disimpan.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithPdfCompliance_out.pdf", options);
```

### Lihat Juga

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


