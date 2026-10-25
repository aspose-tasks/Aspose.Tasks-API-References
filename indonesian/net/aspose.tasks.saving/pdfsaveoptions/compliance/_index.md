---
title: "PdfSaveOptions.Compliance"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PdfSaveOptions. Mendapatkan atau mengatur tingkat kepatuhan yang diinginkan untuk dokumen PDF yang dihasilkan. Defaultnya adalah Pdf15"
type: docs
weight: 20
url: /id/net/aspose.tasks.saving/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Mendapatkan atau mengatur tingkat kepatuhan yang diinginkan untuk dokumen PDF yang dihasilkan. Defaultnya adalah Pdf15.

```csharp
public PdfCompliance Compliance { get; set; }
```

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

* enum [PdfCompliance](../../pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


