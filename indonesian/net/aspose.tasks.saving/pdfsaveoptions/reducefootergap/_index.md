---
title: "PdfSaveOptions.ReduceFooterGap"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PdfSaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi"
type: docs
weight: 80
url: /id/net/aspose.tasks.saving/pdfsaveoptions/reducefootergap/
---
## PdfSaveOptions.ReduceFooterGap property

Mendapatkan atau mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Contoh

Menampilkan cara mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi dalam file output PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions { ReduceFooterGap = true, PageSize = PageSize.A0, Timescale = Timescale.Days };

project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.pdf", options);
```

### Lihat Juga

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


