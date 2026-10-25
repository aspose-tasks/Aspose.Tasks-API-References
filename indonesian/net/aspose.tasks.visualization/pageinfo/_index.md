---
title: "Kelas PageInfo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.PageInfo. Mewakili data pengaturan halaman yang ada dalam format file MPP dan digunakan untuk pencetakan."
type: docs
weight: 3200
url: /id/net/aspose.tasks.visualization/pageinfo/
---
## PageInfo class

Mewakili data pengaturan halaman yang ada dalam format file MPP dan digunakan untuk pencetakan.

```csharp
public class PageInfo
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PageInfo](pageinfo/)() | Menginisialisasi instance baru dari kelas `PageInfo`. Mewakili data pengaturan halaman yang ada dalam format file MPP dan digunakan untuk pencetakan. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Footer](../../aspose.tasks.visualization/pageinfo/footer/) { get; set; } | Mendapatkan atau mengatur sebuah instance dari kelas [`HeaderFooterInfo`](../headerfooterinfo/) yang mewakili data footer. |
| [Header](../../aspose.tasks.visualization/pageinfo/header/) { get; set; } | Mendapatkan atau mengatur instance dari kelas [`HeaderFooterInfo`](../headerfooterinfo/) yang mewakili data header. |
| [Legend](../../aspose.tasks.visualization/pageinfo/legend/) { get; set; } | Mendapatkan atau mengatur sebuah instance dari kelas [`PageLegend`](../pagelegend/) yang menentukan opsi rendering legenda halaman. |
| [Margins](../../aspose.tasks.visualization/pageinfo/margins/) { get; } | Mendapatkan sebuah instance dari kelas [`PageMargins`](../pagemargins/) yang menentukan margin halaman. |
| [Name](../../aspose.tasks.visualization/pageinfo/name/) { get; } | Mendapatkan nama tampilan yang data pengaturannya digunakan. |
| [PageSettings](../../aspose.tasks.visualization/pageinfo/pagesettings/) { get; } | Mendapatkan sebuah instance dari kelas [`PageSettings`](./pagesettings/) yang menentukan pengaturan pencetakan halaman. |
| [PageViewSettings](../../aspose.tasks.visualization/pageinfo/pageviewsettings/) { get; } | Mendapatkan sebuah instance dari kelas [`PageViewSettings`](./pageviewsettings/) yang menentukan pengaturan pencetakan tampilan halaman. |

## Contoh

Menampilkan cara bekerja dengan informasi halaman pada tampilan MS Project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// memungkinkan memodifikasi tampilan default
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// memungkinkan memodifikasi margin
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// mari mengubah pengaturan halaman
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// mari mengubah pengaturan tampilan halaman
// atur nilai yang menunjukkan apakah catatan harus dicetak.
info.PageViewSettings.PrintNotes = true;

var header = new HeaderFooterInfo
{
    LeftText = "Left header text",
    CenteredText = "Centered header text",
    RightText = "Right header text"
};
var legend = new PageLegend
{
    LeftText =  "Left legend text",
    CenteredText = "Centered legend text",
    RightText = "Right legend text"
};
var footer = new HeaderFooterInfo
{
    LeftText = "Left footer text",
    CenteredText = "Centered footer text",
    RightText = "Right footer text"
};

info.Header = header;
info.Legend = legend;
info.Footer = footer;

// bekerja dengan proyek...
```

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


