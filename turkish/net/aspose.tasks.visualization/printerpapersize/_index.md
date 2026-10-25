---
title: "Enum PrinterPaperSize"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.PrinterPaperSize enum. Baskı için kullanılan kağıt boyutunu belirtir."
type: docs
weight: 3280
url: /tr/net/aspose.tasks.visualization/printerpapersize/
---
## PrinterPaperSize enumeration

Yazdırma için kullanılan kağıt boyutunu belirtir.

```csharp
public enum PrinterPaperSize
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Custom | `1` | Kağıt boyutunun kullanıcı tarafından tanımlandığını gösterir. |
| PaperLetter | `1` | Zarf Mektup yazıcı kağıt boyutunu (8.5 in. by 11 in.) gösterir. |
| PaperLetterSmall | `2` | Küçük Mektup yazıcı kağıt boyutunu (8.5 in. by 11 in.) gösterir. |
| PaperTabloid | `3` | Tabloid yazıcı kağıt boyutunu (11 in. by 17 in.) gösterir. |
| PaperLedger | `4` | Ledger yazıcı kağıt boyutunu (17 in. by 11 in.) gösterir. |
| PaperLegal | `5` | Zarf yasal yazıcı kağıt boyutunu (8.5 in. by 14 in.) gösterir. |
| PaperStatement | `6` | Statement yazıcı kağıt boyutunu (5.5 in. by 8.5 in.) gösterir. |
| PaperExecutive | `7` | Zarf yönetici yazıcı kağıt boyutunu (7.25 in. by 10.5 in.) gösterir. |
| PaperA3 | `8` | A3 yazıcı kağıt boyutunu (297 mm by 420 mm) gösterir. |
| PaperA4 | `9` | A4 yazıcı kağıt boyutunu (210 mm by 297 mm) gösterir. |
| PaperA4Small | `10` | Küçük A4 yazıcı kağıt boyutunu (210 mm by 297 mm) gösterir. |
| PaperA5 | `11` | A5 yazıcı kağıt boyutunu (148 mm by 210 mm) gösterir. |
| PaperB4 | `12` | B4 yazıcı kağıt boyutunu (250 mm by 353 mm) gösterir. |
| PaperB5 | `13` | B5 yazıcı kağıt boyutunu (176 mm by 250 mm) gösterir. |
| PaperFolio | `14` | Folio yazıcı kağıt boyutunu (8.5 in. by 13 in.) gösterir. |
| PaperQuarto | `15` | Quarto yazıcı kağıt boyutunu (215 mm by 275 mm) gösterir. |
| PaperStandard10x14 | `16` | Standart yazıcı kağıt boyutunu (10 in. by 14 in.) gösterir. |
| PaperStandard11x17 | `17` | Standart yazıcı kağıt boyutunu (11 in. by 17 in.) gösterir. |
| PaperNote | `18` | Not yazıcı kağıt boyutunu (8.5 in. by 11 in.) gösterir. |
| PaperEnvelope10 | `20` | Zarf10 yazıcı kağıt boyutunu (4.125 in. by 9.5 in.) gösterir. |
| PaperCSheet | `24` | C paper yazıcı kağıt boyutunu (17 in. by 22 in.) gösterir. |
| PaperDSheet | `25` | D paper yazıcı kağıt boyutunu (22 in. by 34 in.) gösterir. |
| PaperESheet | `26` | E paper yazıcı kağıt boyutunu (34 in. by 44 in.) gösterir. |
| PaperEnvelopeMonarch | `37` | Zarf Monarch yazıcı kağıt boyutunu (3.875 in. by 7.5 in.) gösterir. |
| PaperStandard9x11 | `44` | Standart yazıcı kağıt boyutunu (9 in. by 11 in.) gösterir. |
| PaperStandard10x11 | `45` | Standart yazıcı kağıt boyutunu (10 in. by 11 in.) gösterir. |
| PaperStandard15x11 | `46` | Standart yazıcı kağıdı boyutunu (15 inç x 11 inç) gösterir. |
| PaperA2 | `66` | A2 yazıcı kağıdı boyutunu (420 mm x 594 mm) gösterir. |

## Örnekler

MS Project görünümünün sayfa bilgileriyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// varsayılan görünümü değiştirelim
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// kenar boşluklarını değiştirelim
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// sayfa ayarlarını değiştirelim
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// sayfa görünüm ayarlarını değiştirelim
// Notların yazdırılıp yazdırılmayacağını gösteren bir değeri ayarlar.
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

// projeyle çalış...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


