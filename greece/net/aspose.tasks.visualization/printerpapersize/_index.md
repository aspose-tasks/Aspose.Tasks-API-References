---
title: "Απαρίθμηση PrinterPaperSize"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.Visualization.PrinterPaperSize. Καθορίζει το μέγεθος χαρτιού που χρησιμοποιείται για εκτύπωση"
type: docs
weight: 3280
url: /el/net/aspose.tasks.visualization/printerpapersize/
---
## PrinterPaperSize enumeration

Καθορίζει το μέγεθος χαρτιού που χρησιμοποιείται για εκτύπωση.

```csharp
public enum PrinterPaperSize
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Custom | `1` | Δηλώνει ότι το μέγεθος χαρτιού ορίζεται από τον χρήστη. |
| PaperLetter | `1` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Envelope Letter (8.5 ίν. x 11 ίν.). |
| PaperLetterSmall | `2` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Small Letter (8.5 ίν. x 11 ίν.). |
| PaperTabloid | `3` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Tabloid (11 ίν. x 17 ίν.). |
| PaperLedger | `4` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Ledger (17 ίν. x 11 ίν.). |
| PaperLegal | `5` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Envelope legal (8.5 ίν. x 14 ίν.). |
| PaperStatement | `6` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Statement (5.5 ίν. x 8.5 ίν.). |
| PaperExecutive | `7` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Envelope executive (7.25 ίν. x 10.5 ίν.). |
| PaperA3 | `8` | Δείχνει το μέγεθος χαρτιού εκτυπωτή A3 (297 χλμ x 420 χλμ). |
| PaperA4 | `9` | Δείχνει το μέγεθος χαρτιού εκτυπωτή A4 (210 χλμ x 297 χλμ). |
| PaperA4Small | `10` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Small A4 (210 χλμ x 297 χλμ). |
| PaperA5 | `11` | Δείχνει το μέγεθος χαρτιού εκτυπωτή A5 (148 χλμ x 210 χλμ). |
| PaperB4 | `12` | Δείχνει το μέγεθος χαρτιού εκτυπωτή B4 (250 χλμ x 353 χλμ). |
| PaperB5 | `13` | Δείχνει το μέγεθος χαρτιού εκτυπωτή B5 (176 χλμ x 250 χλμ). |
| PaperFolio | `14` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Folio (8.5 ίν. x 13 ίν.). |
| PaperQuarto | `15` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Quarto (215 χλμ x 275 χλμ). |
| PaperStandard10x14 | `16` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Standard (10 ίν. x 14 ίν.). |
| PaperStandard11x17 | `17` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Standard (11 ίν. x 17 ίν.). |
| PaperNote | `18` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Note (8.5 ίν. x 11 ίν.). |
| PaperEnvelope10 | `20` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Envelope10 (4.125 ίν. x 9.5 ίν.). |
| PaperCSheet | `24` | Δείχνει το μέγεθος χαρτιού εκτυπωτή C paper (17 ίν. x 22 ίν.). |
| PaperDSheet | `25` | Δείχνει το μέγεθος χαρτιού εκτυπωτή D paper (22 ίν. x 34 ίν.). |
| PaperESheet | `26` | Δείχνει το μέγεθος χαρτιού εκτυπωτή E paper (34 ίν. x 44 ίν.). |
| PaperEnvelopeMonarch | `37` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Envelope Monarch (3.875 ίν. x 7.5 ίν.). |
| PaperStandard9x11 | `44` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Standard (9 ίν. x 11 ίν.). |
| PaperStandard10x11 | `45` | Δείχνει το μέγεθος χαρτιού εκτυπωτή Standard (10 ίν. x 11 ίν.). |
| PaperStandard15x11 | `46` | Δείχνει το τυπικό μέγεθος χαρτιού εκτυπωτή (15 ίντσες επί 11 ίντσες). |
| PaperA2 | `66` | Δείχνει το μέγεθος χαρτιού εκτυπωτή A2 (420 χλμ επί 594 χλμ). |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τις πληροφορίες σελίδας της προβολής MS Project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// επιτρέπει την τροποποίηση της προεπιλεγμένης προβολής
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// επιτρέπει την τροποποίηση των περιθωρίων
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// Ας τροποποιήσουμε τις ρυθμίσεις σελίδας.
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// Ας τροποποιήσουμε τις ρυθμίσεις προβολής σελίδας.
// ορίστε μια τιμή που υποδεικνύει εάν θα εκτυπωθούν σημειώσεις.
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

// εργαστείτε με το έργο...
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


