---
title: "PageSettings.FirstPageNumber"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PageSettings. Mendapatkan atau mengatur nomor halaman pertama untuk pencetakan."
type: docs
weight: 30
url: /id/net/aspose.tasks.visualization/pagesettings/firstpagenumber/
---
## PageSettings.FirstPageNumber property

Mendapatkan atau mengatur nomor halaman pertama untuk pencetakan.

```csharp
public short FirstPageNumber { get; set; }
```

## Contoh

Menampilkan cara bekerja dengan &lt;see cref="Aspose.Tasks.Visualization.PageSettings" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// dapatkan pengaturan
var settings = project.DefaultView.PageInfo.PageSettings;
// mari atur beberapa properti
// atur nilai yang menunjukkan apakah orientasi halaman potret; mengembalikan false jika orientasi halaman lanskap.
settings.IsPortrait = true;
// atur jumlah halaman dalam lebar yang akan dicetak.
settings.PagesInWidth = 5;
// atur jumlah halaman dalam tinggi yang akan dicetak.
settings.PagesInHeight = 7;
// atur persentase ukuran normal untuk menyesuaikan pencetakan.
settings.PercentOfNormalSize = 200;
// atur ukuran kertas. Bisa menjadi salah satu nilai dari enumerasi <see cref="T:Aspose.Tasks.Visualization.PrinterPaperSize" />.
settings.PaperSize = PrinterPaperSize.PaperB4;
// atur nomor halaman pertama untuk pencetakan.
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

### Lihat Juga

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


