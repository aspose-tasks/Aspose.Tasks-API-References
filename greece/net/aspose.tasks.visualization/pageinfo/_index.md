---
title: "Κλάση PageInfo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Visualization.PageInfo. Αντιπροσωπεύει δεδομένα ρύθμισης σελίδας που υπάρχουν στη μορφή αρχείου MPP και χρησιμοποιούνται για εκτύπωση."
type: docs
weight: 3200
url: /el/net/aspose.tasks.visualization/pageinfo/
---
## PageInfo class

Αναπαριστά δεδομένα ρύθμισης σελίδας που υπάρχουν στη μορφή αρχείου MPP και χρησιμοποιούνται για εκτύπωση.

```csharp
public class PageInfo
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PageInfo](pageinfo/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `PageInfo`. Αντιπροσωπεύει δεδομένα ρύθμισης σελίδας που υπάρχουν στη μορφή αρχείου MPP και χρησιμοποιούνται για εκτύπωση. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Footer](../../aspose.tasks.visualization/pageinfo/footer/) { get; set; } | Λαμβάνει ή ορίζει μια παρουσία της κλάσης [`HeaderFooterInfo`](../headerfooterinfo/) που αντιπροσωπεύει δεδομένα υποσέλιδου. |
| [Header](../../aspose.tasks.visualization/pageinfo/header/) { get; set; } | Λαμβάνει ή ορίζει την παρουσία της κλάσης [`HeaderFooterInfo`](../headerfooterinfo/) που αντιπροσωπεύει δεδομένα κεφαλίδας. |
| [Legend](../../aspose.tasks.visualization/pageinfo/legend/) { get; set; } | Λαμβάνει ή ορίζει μια παρουσία της κλάσης [`PageLegend`](../pagelegend/) που καθορίζει επιλογές απόδοσης του υπομνήματος σελίδας. |
| [Margins](../../aspose.tasks.visualization/pageinfo/margins/) { get; } | Λαμβάνει μια παρουσία της κλάσης [`PageMargins`](../pagemargins/) που καθορίζει τα περιθώρια της σελίδας. |
| [Name](../../aspose.tasks.visualization/pageinfo/name/) { get; } | Λαμβάνει το όνομα της προβολής για την οποία χρησιμοποιούνται τα δεδομένα ρύθμισης. |
| [PageSettings](../../aspose.tasks.visualization/pageinfo/pagesettings/) { get; } | Λαμβάνει μια παρουσία της κλάσης [`PageSettings`](./pagesettings/) που καθορίζει τις ρυθμίσεις εκτύπωσης σελίδας. |
| [PageViewSettings](../../aspose.tasks.visualization/pageinfo/pageviewsettings/) { get; } | Λαμβάνει μια παρουσία της κλάσης [`PageViewSettings`](./pageviewsettings/) που καθορίζει τις ρυθμίσεις εκτύπωσης προβολής σελίδας. |

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


