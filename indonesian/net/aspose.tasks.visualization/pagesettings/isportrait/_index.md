---
title: "PageSettings.IsPortrait"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PageSettings. Mendapatkan atau mengatur nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape."
type: docs
weight: 40
url: /id/net/aspose.tasks.visualization/pagesettings/isportrait/
---
## PageSettings.IsPortrait property

Mendapatkan atau mengatur nilai yang menunjukkan apakah orientasi halaman potret; mengembalikan false jika orientasi halaman lanskap.

```csharp
public bool IsPortrait { get; set; }
```

## Catatan

Berlaku selama proses rendering ketika SaveOptions.PageSize == Visualization.PageSize.DefinedInView.

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

Menampilkan cara menentukan ukuran halaman dan orientasi menggunakan pengaturan View atau menggunakan SaveOptions.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// Dalam kasus ini ukuran halaman dan orientasi diterapkan dari properti view.PageInfo.PageSettings.PaperSize dan view.PageInfo.PageSettings.IsPortrait.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// Dalam kasus ini ukuran halaman dan orientasi diterapkan dari properti SaveOptions.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// Dalam kasus ini ukuran halaman diterapkan dari SaveOptions.CustomPageSize. Properti IsPortrait tidak dipertimbangkan.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### Lihat Juga

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


