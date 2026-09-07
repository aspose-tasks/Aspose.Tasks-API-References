---
title: "HtmlSaveOptions.ReduceFooterGap"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti HtmlSaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi"
type: docs
weight: 150
url: /id/net/aspose.tasks.saving/htmlsaveoptions/reducefootergap/
---
## HtmlSaveOptions.ReduceFooterGap property

Mendapatkan atau mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Contoh

Menampilkan cara mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi dalam file output HTML.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      ReduceFooterGap = true,
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A0,
                      Timescale = Timescale.Days
                  };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.html", options);
```

### Lihat Juga

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


