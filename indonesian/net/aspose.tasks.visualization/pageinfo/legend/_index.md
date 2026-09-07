---
title: "PageInfo.Legend"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PageInfo. Mendapatkan atau mengatur instance dari kelas PageLegend yang menentukan opsi rendering legenda halaman"
type: docs
weight: 40
url: /id/net/aspose.tasks.visualization/pageinfo/legend/
---
## PageInfo.Legend property

Mendapatkan atau mengatur instance dari kelas [`PageLegend`](../../pagelegend/) yang menentukan opsi rendering legenda halaman.

```csharp
public PageLegend Legend { get; set; }
```

## Catatan

Saat ini hanya berlaku untuk tampilan Gantt Chart.

## Contoh

Menampilkan cara bekerja dengan informasi legenda halaman.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// mari membaca informasi legenda halaman
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// modifikasi legenda juga didukung
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

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

* class [PageLegend](../../pagelegend/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


