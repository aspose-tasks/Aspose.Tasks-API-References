---
title: "PageInfo.PageInfo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor PageInfo. Menginisialisasi instance baru dari kelas PageInfo. Mewakili data penyiapan halaman yang ada dalam format file MPP dan digunakan untuk pencetakan"
type: docs
weight: 10
url: /id/net/aspose.tasks.visualization/pageinfo/pageinfo/
---
## PageInfo constructor

Menginisialisasi instance baru dari kelas [`PageInfo`](../). Mewakili data penyiapan halaman yang ada dalam format file MPP dan digunakan untuk pencetakan.

```csharp
public PageInfo()
```

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

* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


