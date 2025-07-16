---
title: Enum PrinterPaperSize
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.PrinterPaperSize enum. Specifies the paper size which is used for printing
type: docs
weight: 3200
url: /net/aspose.tasks.visualization/printerpapersize/
---
## PrinterPaperSize enumeration

Specifies the paper size which is used for printing.

```csharp
public enum PrinterPaperSize
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Custom | `1` | Indicates that the paper size is defined by the user. |
| PaperLetter | `1` | Indicates Envelope Letter printer paper size (8.5 in. by 11 in.). |
| PaperLetterSmall | `2` | Indicates Small Letter printer paper size (8.5 in. by 11 in.). |
| PaperTabloid | `3` | Indicates Tabloid printer paper size (11 in. by 17 in.). |
| PaperLedger | `4` | Indicates Ledger printer paper size (17 in. by 11 in.). |
| PaperLegal | `5` | Indicates Envelope legal printer paper size (8.5 in. by 14 in.). |
| PaperStatement | `6` | Indicates Statement printer paper size (5.5 in. by 8.5 in.). |
| PaperExecutive | `7` | Indicates Envelope executive printer paper size (7.25 in. by 10.5 in.). |
| PaperA3 | `8` | Indicates A3 printer paper size (297 mm by 420 mm). |
| PaperA4 | `9` | Indicates A4 printer paper size (210 mm by 297 mm). |
| PaperA4Small | `10` | Indicates Small A4 printer paper size (210 mm by 297 mm). |
| PaperA5 | `11` | Indicates A5 printer paper size (148 mm by 210 mm). |
| PaperB4 | `12` | Indicates B4 printer paper size (250 mm by 353 mm). |
| PaperB5 | `13` | Indicates B5 printer paper size (176 mm by 250 mm). |
| PaperFolio | `14` | Indicates Folio printer paper size (8.5 in. by 13 in.). |
| PaperQuarto | `15` | Indicates Quarto printer paper size (215 mm by 275 mm). |
| PaperStandard10x14 | `16` | Indicates Standard printer paper size (10 in. by 14 in.). |
| PaperStandard11x17 | `17` | Indicates Standard printer paper size (11 in. by 17 in.). |
| PaperNote | `18` | Indicates Note printer paper size (8.5 in. by 11 in.). |
| PaperEnvelope10 | `20` | Indicates Envelope10 printer paper size (4.125 in. by 9.5 in.). |
| PaperCSheet | `24` | Indicates C paper printer paper size (17 in. by 22 in.). |
| PaperDSheet | `25` | Indicates D paper printer paper size (22 in. by 34 in.). |
| PaperESheet | `26` | Indicates E paper printer paper size (34 in. by 44 in.). |
| PaperEnvelopeMonarch | `37` | Indicates Envelope Monarch printer paper size (3.875 in. by 7.5 in.). |
| PaperStandard9x11 | `44` | Indicates Standard printer paper size (9 in. by 11 in.). |
| PaperStandard10x11 | `45` | Indicates Standard printer paper size (10 in. by 11 in.). |
| PaperStandard15x11 | `46` | Indicates Standard printer paper size (15 in. by 11 in.). |
| PaperA2 | `66` | Indicates A2 printer paper size (420 mm by 594 mm). |

## Examples

Shows how to work with page info of MS Project view.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// lets modify the default view
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// lets modify margins
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// lets modify page settings
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// lets modify page view settings
// set a value indicating whether to print notes.
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

// work with project...
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


