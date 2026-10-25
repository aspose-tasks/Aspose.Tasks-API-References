---
title: "PageSettings.IsPortrait"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PageSettings. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν η προσανατολισμός της σελίδας είναι πορτραίτο· επιστρέφει false αν η προσανατολισμός της σελίδας είναι τοπίο"
type: docs
weight: 40
url: /el/net/aspose.tasks.visualization/pagesettings/isportrait/
---
## PageSettings.IsPortrait property

Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν ο προσανατολισμός της σελίδας είναι πορτραίτο· επιστρέφει false εάν ο προσανατολισμός της σελίδας είναι τοπίο.

```csharp
public bool IsPortrait { get; set; }
```

## Παρατηρήσεις

Είναι εφαρμόσιμο κατά την απόδοση όταν SaveOptions.PageSize == Visualization.PageSize.DefinedInView.

## Παραδείγματα

Δείχνει πώς να εργαστείτε με &lt;see cref=\"Aspose.Tasks.Visualization.PageSettings\" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// λάβετε τις ρυθμίσεις
var settings = project.DefaultView.PageInfo.PageSettings;
// ας ρυθμίσουμε κάποιες ιδιότητες
// ορίστε μια τιμή που υποδεικνύει εάν ο προσανατολισμός της σελίδας είναι πορτραίτο· επιστρέφει false εάν ο προσανατολισμός της σελίδας είναι τοπίο.
settings.IsPortrait = true;
// ορίστε τον αριθμό των σελίδων σε πλάτος που θα εκτυπωθούν.
settings.PagesInWidth = 5;
// ορίστε τον αριθμό των σελίδων σε ύψος που θα εκτυπωθούν.
settings.PagesInHeight = 7;
// ορίστε ένα ποσοστό του κανονικού μεγέθους για προσαρμογή της εκτύπωσης.
settings.PercentOfNormalSize = 200;
// ορίστε ένα μέγεθος χαρτιού. Μπορεί να είναι μία από τις τιμές της απαρίθμησης <see cref=\"T:Aspose.Tasks.Visualization.PrinterPaperSize\" />.
settings.PaperSize = PrinterPaperSize.PaperB4;
// ορίστε τον αριθμό της πρώτης σελίδας για εκτύπωση.
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

Δείχνει πώς να καθορίσετε το μέγεθος και τον προσανατολισμό της σελίδας χρησιμοποιώντας τις ρυθμίσεις View ή χρησιμοποιώντας το SaveOptions.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// Σε αυτήν την περίπτωση το μέγεθος και ο προσανατολισμός της σελίδας εφαρμόζονται από τις ιδιότητες view.PageInfo.PageSettings.PaperSize και view.PageInfo.PageSettings.IsPortrait.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// Σε αυτήν την περίπτωση το μέγεθος και ο προσανατολισμός της σελίδας εφαρμόζονται από τις ιδιότητες του SaveOptions.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// Σε αυτήν την περίπτωση το μέγεθος της σελίδας εφαρμόζεται από το SaveOptions.CustomPageSize. Η ιδιότητα IsPortrait δεν λαμβάνεται υπόψη.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### Δείτε επίσης

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


