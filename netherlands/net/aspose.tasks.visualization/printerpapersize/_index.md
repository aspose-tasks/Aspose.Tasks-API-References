---
title: "Enum PrinterPaperSize"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.PrinterPaperSize-enum. Specificeert de papiergrootte die wordt gebruikt voor afdrukken."
type: docs
weight: 3280
url: /nl/net/aspose.tasks.visualization/printerpapersize/
---
## PrinterPaperSize enumeration

Specificeert de papiergrootte die wordt gebruikt voor afdrukken.

```csharp
public enum PrinterPaperSize
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Custom | `1` | Geeft aan dat de papiergrootte door de gebruiker is gedefinieerd. |
| PaperLetter | `1` | Geeft aan Envelop Letter printerpapierformaat (8.5 in. bij 11 in.). |
| PaperLetterSmall | `2` | Geeft aan Kleine Letter printerpapierformaat (8.5 in. bij 11 in.). |
| PaperTabloid | `3` | Geeft aan Tabloid printerpapierformaat (11 in. bij 17 in.). |
| PaperLedger | `4` | Geeft aan Ledger printerpapierformaat (17 in. bij 11 in.). |
| PaperLegal | `5` | Geeft aan Envelop legal printerpapierformaat (8.5 in. bij 14 in.). |
| PaperStatement | `6` | Geeft aan Statement printerpapierformaat (5.5 in. bij 8.5 in.). |
| PaperExecutive | `7` | Geeft aan Envelop executive printerpapierformaat (7.25 in. bij 10.5 in.). |
| PaperA3 | `8` | Geeft aan A3 printerpapierformaat (297 mm bij 420 mm). |
| PaperA4 | `9` | Geeft aan A4 printerpapierformaat (210 mm bij 297 mm). |
| PaperA4Small | `10` | Geeft aan Kleine A4 printerpapierformaat (210 mm bij 297 mm). |
| PaperA5 | `11` | Geeft aan A5 printerpapierformaat (148 mm bij 210 mm). |
| PaperB4 | `12` | Geeft aan B4 printerpapierformaat (250 mm bij 353 mm). |
| PaperB5 | `13` | Geeft aan B5 printerpapierformaat (176 mm bij 250 mm). |
| PaperFolio | `14` | Geeft aan Folio printerpapierformaat (8.5 in. bij 13 in.). |
| PaperQuarto | `15` | Geeft aan Quarto printerpapierformaat (215 mm bij 275 mm). |
| PaperStandard10x14 | `16` | Geeft aan Standaard printerpapierformaat (10 in. bij 14 in.). |
| PaperStandard11x17 | `17` | Geeft aan Standaard printerpapierformaat (11 in. bij 17 in.). |
| PaperNote | `18` | Geeft aan Notitie printerpapierformaat (8.5 in. bij 11 in.). |
| PaperEnvelope10 | `20` | Geeft aan Envelop10 printerpapierformaat (4.125 in. bij 9.5 in.). |
| PaperCSheet | `24` | Geeft aan C-papier printerpapierformaat (17 in. bij 22 in.). |
| PaperDSheet | `25` | Geeft aan D-papier printerpapierformaat (22 in. bij 34 in.). |
| PaperESheet | `26` | Geeft aan E-papier printerpapierformaat (34 in. bij 44 in.). |
| PaperEnvelopeMonarch | `37` | Geeft aan Envelop Monarch printerpapierformaat (3.875 in. bij 7.5 in.). |
| PaperStandard9x11 | `44` | Geeft aan Standaard printerpapierformaat (9 in. bij 11 in.). |
| PaperStandard10x11 | `45` | Geeft aan Standaard printerpapierformaat (10 in. bij 11 in.). |
| PaperStandard15x11 | `46` | Geeft de standaard printerpapiergrootte aan (15 inch bij 11 inch). |
| PaperA2 | `66` | Geeft de A2 printerpapiergrootte aan (420 mm bij 594 mm). |

## Voorbeelden

Toont hoe te werken met paginainformatie van de MS Project-weergave.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// laat de standaardweergave aanpassen
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// laat marges aanpassen
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// laten we paginainstellingen wijzigen
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// laten we paginaviewinstellingen wijzigen
// stel een waarde in die aangeeft of notities moeten worden afgedrukt.
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

// werken met project...
```

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


