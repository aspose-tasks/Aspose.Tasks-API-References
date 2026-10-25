---
title: "PageInfo.Legend"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PageInfo. Λαμβάνει ή ορίζει μια παρουσία της κλάσης PageLegend που καθορίζει τις επιλογές απόδοσης του υπομνήματος σελίδας"
type: docs
weight: 40
url: /el/net/aspose.tasks.visualization/pageinfo/legend/
---
## PageInfo.Legend property

Λαμβάνει ή ορίζει μια παρουσία της κλάσης [`PageLegend`](../../pagelegend/) που καθορίζει τις επιλογές απόδοσης του υπομνήματος σελίδας.

```csharp
public PageLegend Legend { get; set; }
```

## Παρατηρήσεις

Προς το παρόν ισχύει μόνο για προβολές Gantt Chart.

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τις πληροφορίες του υπομνήματος σελίδας.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Ας διαβάσουμε τις πληροφορίες του υπομνήματος σελίδας.
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// Επίσης υποστηρίζεται η τροποποίηση ενός υπομνήματος.
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

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

* class [PageLegend](../../pagelegend/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


