---
title: "PageInfo.Name"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PageInfo. Λαμβάνει το όνομα της προβολής για την οποία χρησιμοποιούνται τα δεδομένα ρύθμισης"
type: docs
weight: 60
url: /el/net/aspose.tasks.visualization/pageinfo/name/
---
## PageInfo.Name property

Λαμβάνει το όνομα της προβολής για την οποία χρησιμοποιούνται τα δεδομένα ρύθμισης.

```csharp
public string Name { get; }
```

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

* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


