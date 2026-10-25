---
title: "PageInfo.PageSettings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PageInfo. Mendapatkan instance dari kelas PageSettings yang menentukan pengaturan pencetakan halaman"
type: docs
weight: 70
url: /id/net/aspose.tasks.visualization/pageinfo/pagesettings/
---
## PageInfo.PageSettings property

Mendapatkan instance dari kelas `PageSettings` yang menentukan pengaturan pencetakan halaman.

```csharp
public PageSettings PageSettings { get; }
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

* class [PageSettings](../../pagesettings/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


