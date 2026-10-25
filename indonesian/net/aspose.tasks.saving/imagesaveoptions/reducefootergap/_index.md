---
title: "ImageSaveOptions.ReduceFooterGap"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ImageSaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi"
type: docs
weight: 80
url: /id/net/aspose.tasks.saving/imagesaveoptions/reducefootergap/
---
## ImageSaveOptions.ReduceFooterGap property

Mendapatkan atau mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Contoh

Menampilkan cara mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Gunakan properti ReduceFooterGap untuk mengurangi celah antara daftar tugas dan Footer
var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png)
                           {
                               ReduceFooterGap = true, /* set to true */ 
                               RenderToSinglePage = false,
                               PageSize = PageSize.A0,
                               Timescale = Timescale.Days
                           };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.png", imageSaveOptions);
```

### Lihat Juga

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


