---
title: "SaveOptions.CustomPageSize"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur ukuran halaman khusus dalam poin, 1 poin = 1/72 inci."
type: docs
weight: 20
url: /id/net/aspose.tasks.saving/saveoptions/custompagesize/
---
## SaveOptions.CustomPageSize property

Mendapatkan atau mengatur ukuran halaman khusus dalam poin (1 poin = 1/72 inci).

```csharp
public SizeF CustomPageSize { get; set; }
```

## Contoh

Menampilkan cara mengatur ukuran halaman khusus ketika proyek disimpan ke PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.GanttChart;
options.CustomPageSize = new SizeF(5.8F * 72, 8.3F * 72);

project.Save(OutDir + "WorkWithCustomPageSize_out.pdf", options);
```

### Lihat Juga

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


