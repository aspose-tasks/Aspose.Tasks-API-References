---
title: "Enum PrinterPaperSize"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Visualization.PrinterPaperSize. Menentukan ukuran kertas yang digunakan untuk pencetakan."
type: docs
weight: 3280
url: /id/net/aspose.tasks.visualization/printerpapersize/
---
## PrinterPaperSize enumeration

Menentukan ukuran kertas yang digunakan untuk pencetakan.

```csharp
public enum PrinterPaperSize
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Custom | `1` | Menunjukkan bahwa ukuran kertas didefinisikan oleh pengguna. |
| PaperLetter | `1` | Menunjukkan ukuran kertas printer Amplop Letter (8.5 in. by 11 in.). |
| PaperLetterSmall | `2` | Menunjukkan ukuran kertas printer Letter Kecil (8.5 in. by 11 in.). |
| PaperTabloid | `3` | Menunjukkan ukuran kertas printer Tabloid (11 in. by 17 in.). |
| PaperLedger | `4` | Menunjukkan ukuran kertas printer Ledger (17 in. by 11 in.). |
| PaperLegal | `5` | Menunjukkan ukuran kertas printer Amplop legal (8.5 in. by 14 in.). |
| PaperStatement | `6` | Menunjukkan ukuran kertas printer Statement (5.5 in. by 8.5 in.). |
| PaperExecutive | `7` | Menunjukkan ukuran kertas printer Amplop eksekutif (7.25 in. by 10.5 in.). |
| PaperA3 | `8` | Menunjukkan ukuran kertas printer A3 (297 mm by 420 mm). |
| PaperA4 | `9` | Menunjukkan ukuran kertas printer A4 (210 mm by 297 mm). |
| PaperA4Small | `10` | Menunjukkan ukuran kertas printer A4 Kecil (210 mm by 297 mm). |
| PaperA5 | `11` | Menunjukkan ukuran kertas printer A5 (148 mm by 210 mm). |
| PaperB4 | `12` | Menunjukkan ukuran kertas printer B4 (250 mm by 353 mm). |
| PaperB5 | `13` | Menunjukkan ukuran kertas printer B5 (176 mm by 250 mm). |
| PaperFolio | `14` | Menunjukkan ukuran kertas printer Folio (8.5 in. by 13 in.). |
| PaperQuarto | `15` | Menunjukkan ukuran kertas printer Quarto (215 mm by 275 mm). |
| PaperStandard10x14 | `16` | Menunjukkan ukuran kertas printer Standar (10 in. by 14 in.). |
| PaperStandard11x17 | `17` | Menunjukkan ukuran kertas printer Standar (11 in. by 17 in.). |
| PaperNote | `18` | Menunjukkan ukuran kertas printer Note (8.5 in. by 11 in.). |
| PaperEnvelope10 | `20` | Menunjukkan ukuran kertas printer Amplop10 (4.125 in. by 9.5 in.). |
| PaperCSheet | `24` | Menunjukkan ukuran kertas printer C (17 in. by 22 in.). |
| PaperDSheet | `25` | Menunjukkan ukuran kertas printer D (22 in. by 34 in.). |
| PaperESheet | `26` | Menunjukkan ukuran kertas printer E (34 in. by 44 in.). |
| PaperEnvelopeMonarch | `37` | Menunjukkan ukuran kertas printer Amplop Monarch (3.875 in. by 7.5 in.). |
| PaperStandard9x11 | `44` | Menunjukkan ukuran kertas printer Standar (9 in. by 11 in.). |
| PaperStandard10x11 | `45` | Menunjukkan ukuran kertas printer Standar (10 in. by 11 in.). |
| PaperStandard15x11 | `46` | Menunjukkan ukuran kertas printer Standar (15 in. x 11 in.). |
| PaperA2 | `66` | Menunjukkan ukuran kertas printer A2 (420 mm x 594 mm). |

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


