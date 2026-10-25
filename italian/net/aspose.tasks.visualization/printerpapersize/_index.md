---
title: "Enum PrinterPaperSize"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.Visualization.PrinterPaperSize. Specifica la dimensione della carta utilizzata per la stampa."
type: docs
weight: 3280
url: /it/net/aspose.tasks.visualization/printerpapersize/
---
## PrinterPaperSize enumeration

Specifica la dimensione della carta utilizzata per la stampa.

```csharp
public enum PrinterPaperSize
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Custom | `1` | Indica che la dimensione della carta è definita dall'utente. |
| PaperLetter | `1` | Indica il formato carta per stampante Envelope Letter (8,5 pollici per 11 pollici). |
| PaperLetterSmall | `2` | Indica il formato carta per stampante Small Letter (8,5 pollici per 11 pollici). |
| PaperTabloid | `3` | Indica il formato carta per stampante Tabloid (11 pollici per 17 pollici). |
| PaperLedger | `4` | Indica il formato carta per stampante Ledger (17 pollici per 11 pollici). |
| PaperLegal | `5` | Indica il formato carta per stampante Envelope legal (8,5 pollici per 14 pollici). |
| PaperStatement | `6` | Indica il formato carta per stampante Statement (5,5 pollici per 8,5 pollici). |
| PaperExecutive | `7` | Indica il formato carta per stampante Envelope executive (7,25 pollici per 10,5 pollici). |
| PaperA3 | `8` | Indica il formato carta per stampante A3 (297 mm per 420 mm). |
| PaperA4 | `9` | Indica il formato carta per stampante A4 (210 mm per 297 mm). |
| PaperA4Small | `10` | Indica il formato carta per stampante Small A4 (210 mm per 297 mm). |
| PaperA5 | `11` | Indica il formato carta per stampante A5 (148 mm per 210 mm). |
| PaperB4 | `12` | Indica il formato carta per stampante B4 (250 mm per 353 mm). |
| PaperB5 | `13` | Indica il formato carta per stampante B5 (176 mm per 250 mm). |
| PaperFolio | `14` | Indica il formato carta per stampante Folio (8,5 pollici per 13 pollici). |
| PaperQuarto | `15` | Indica il formato carta per stampante Quarto (215 mm per 275 mm). |
| PaperStandard10x14 | `16` | Indica il formato carta per stampante Standard (10 pollici per 14 pollici). |
| PaperStandard11x17 | `17` | Indica il formato carta per stampante Standard (11 pollici per 17 pollici). |
| PaperNote | `18` | Indica il formato carta per stampante Note (8,5 pollici per 11 pollici). |
| PaperEnvelope10 | `20` | Indica il formato carta per stampante Envelope10 (4,125 pollici per 9,5 pollici). |
| PaperCSheet | `24` | Indica il formato carta per stampante C (17 pollici per 22 pollici). |
| PaperDSheet | `25` | Indica il formato carta per stampante D (22 pollici per 34 pollici). |
| PaperESheet | `26` | Indica il formato carta per stampante E (34 pollici per 44 pollici). |
| PaperEnvelopeMonarch | `37` | Indica il formato carta per stampante Envelope Monarch (3,875 pollici per 7,5 pollici). |
| PaperStandard9x11 | `44` | Indica il formato carta per stampante Standard (9 pollici per 11 pollici). |
| PaperStandard10x11 | `45` | Indica il formato carta per stampante Standard (10 pollici per 11 pollici). |
| PaperStandard15x11 | `46` | Indica la dimensione standard della carta per stampante (15 pollici per 11 pollici). |
| PaperA2 | `66` | Indica la dimensione della carta per stampante A2 (420 mm per 594 mm). |

## Esempi

Mostra come lavorare con le informazioni della pagina nella vista di MS Project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// consente di modificare la vista predefinita
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// consente di modificare i margini
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// consente di modificare le impostazioni della pagina
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// consente di modificare le impostazioni della vista della pagina
// imposta un valore che indica se stampare le note.
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

// lavorare con il progetto...
```

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


