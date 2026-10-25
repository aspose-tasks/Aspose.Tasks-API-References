---
title: "Kelas PageSettings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.PageSettings. Mewakili pengaturan pencetakan untuk satu halaman tampilan proyek"
type: docs
weight: 3240
url: /id/net/aspose.tasks.visualization/pagesettings/
---
## PageSettings class

Mewakili pengaturan pencetakan untuk halaman tampilan proyek.

```csharp
public class PageSettings
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PageSettings](pagesettings/)() | Menginisialisasi instance baru dari kelas `PageSettings`. Mewakili pengaturan pencetakan untuk satu halaman tampilan proyek. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AdjustToPercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menyesuaikan pencetakan ke persentase yang ditentukan ([`PercentOfNormalSize`](./percentofnormalsize/)) dari ukuran normal. |
| [FirstPageNumber](../../aspose.tasks.visualization/pagesettings/firstpagenumber/) { get; set; } | Mendapatkan atau mengatur nomor halaman pertama untuk pencetakan. |
| [IsPortrait](../../aspose.tasks.visualization/pagesettings/isportrait/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah orientasi halaman potret; mengembalikan false jika orientasi halaman lanskap. |
| [PagesInHeight](../../aspose.tasks.visualization/pagesettings/pagesinheight/) { get; set; } | Mendapatkan atau mengatur jumlah halaman dalam tinggi yang akan dicetak. |
| [PagesInWidth](../../aspose.tasks.visualization/pagesettings/pagesinwidth/) { get; set; } | Mendapatkan atau mengatur jumlah halaman dalam lebar yang akan dicetak. |
| [PaperSize](../../aspose.tasks.visualization/pagesettings/papersize/) { get; set; } | Mendapatkan atau mengatur ukuran kertas. Bisa menjadi salah satu nilai dari enumerasi [`PrinterPaperSize`](../printerpapersize/). |
| [PaperSizeId](../../aspose.tasks.visualization/pagesettings/papersizeid/) { get; set; } | Mendapatkan atau mengatur integer yang mewakili salah satu nilai PrinterPaperSize atau ID ukuran halaman khusus. Nilai ini dapat digunakan untuk mendapatkan PaperSize dari pengaturan OS. |
| [PercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/percentofnormalsize/) { get; set; } | Mendapatkan atau mengatur persentase ukuran normal untuk menyesuaikan pencetakan. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


