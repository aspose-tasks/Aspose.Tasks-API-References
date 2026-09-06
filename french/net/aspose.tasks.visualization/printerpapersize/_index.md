---
title: "Enum PrinterPaperSize"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Enum Aspose.Tasks.Visualization.PrinterPaperSize. Spécifie la taille du papier utilisée pour l'impression"
type: docs
weight: 3280
url: /fr/net/aspose.tasks.visualization/printerpapersize/
---
## PrinterPaperSize enumeration

Spécifie la taille du papier utilisée pour l'impression.

```csharp
public enum PrinterPaperSize
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Custom | `1` | Indique que la taille du papier est définie par l'utilisateur. |
| PaperLetter | `1` | Indique la taille du papier d'imprimante Envelope Letter (8.5 in. par 11 in.). |
| PaperLetterSmall | `2` | Indique la taille du papier d'imprimante Small Letter (8.5 in. par 11 in.). |
| PaperTabloid | `3` | Indique la taille du papier d'imprimante Tabloid (11 in. par 17 in.). |
| PaperLedger | `4` | Indique la taille du papier d'imprimante Ledger (17 in. par 11 in.). |
| PaperLegal | `5` | Indique la taille du papier d'imprimante Envelope legal (8.5 in. par 14 in.). |
| PaperStatement | `6` | Indique la taille du papier d'imprimante Statement (5.5 in. par 8.5 in.). |
| PaperExecutive | `7` | Indique la taille du papier d'imprimante Envelope executive (7.25 in. par 10.5 in.). |
| PaperA3 | `8` | Indique la taille du papier d'imprimante A3 (297 mm par 420 mm). |
| PaperA4 | `9` | Indique la taille du papier d'imprimante A4 (210 mm par 297 mm). |
| PaperA4Small | `10` | Indique la taille du papier d'imprimante Small A4 (210 mm par 297 mm). |
| PaperA5 | `11` | Indique la taille du papier d'imprimante A5 (148 mm par 210 mm). |
| PaperB4 | `12` | Indique la taille du papier d'imprimante B4 (250 mm par 353 mm). |
| PaperB5 | `13` | Indique la taille du papier d'imprimante B5 (176 mm par 250 mm). |
| PaperFolio | `14` | Indique la taille du papier d'imprimante Folio (8.5 in. par 13 in.). |
| PaperQuarto | `15` | Indique la taille du papier d'imprimante Quarto (215 mm par 275 mm). |
| PaperStandard10x14 | `16` | Indique la taille du papier d'imprimante Standard (10 in. par 14 in.). |
| PaperStandard11x17 | `17` | Indique la taille du papier d'imprimante Standard (11 in. par 17 in.). |
| PaperNote | `18` | Indique la taille du papier d'imprimante Note (8.5 in. par 11 in.). |
| PaperEnvelope10 | `20` | Indique la taille du papier d'imprimante Envelope10 (4.125 in. par 9.5 in.). |
| PaperCSheet | `24` | Indique la taille du papier d'imprimante C (17 in. par 22 in.). |
| PaperDSheet | `25` | Indique la taille du papier d'imprimante D (22 in. par 34 in.). |
| PaperESheet | `26` | Indique la taille du papier d'imprimante E (34 in. par 44 in.). |
| PaperEnvelopeMonarch | `37` | Indique la taille du papier d'imprimante Envelope Monarch (3.875 in. par 7.5 in.). |
| PaperStandard9x11 | `44` | Indique la taille du papier d'imprimante Standard (9 in. par 11 in.). |
| PaperStandard10x11 | `45` | Indique la taille du papier d'imprimante Standard (10 in. par 11 in.). |
| PaperStandard15x11 | `46` | Indique la taille standard du papier d'imprimante (15 po × 11 po). |
| PaperA2 | `66` | Indique la taille du papier d'imprimante A2 (420 mm × 594 mm). |

## Exemples

Montre comment travailler avec les informations de page de la vue MS Project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// modifions la vue par défaut
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// modifions les marges
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// modifions les paramètres de page
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// modifions les paramètres de vue de page
// définir une valeur indiquant s'il faut imprimer les notes.
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

// travailler avec le projet...
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


