---
title: "PageSettings.PageSettings"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής PageSettings. Αρχικοποιεί μια νέα παρουσία της κλάσης PageSettings. Αντιπροσωπεύει τις ρυθμίσεις εκτύπωσης για μια σελίδα της προβολής έργου."
type: docs
weight: 10
url: /el/net/aspose.tasks.visualization/pagesettings/pagesettings/
---
## PageSettings constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PageSettings`](../). Αντιπροσωπεύει τις ρυθμίσεις εκτύπωσης για μια σελίδα της προβολής έργου.

```csharp
public PageSettings()
```

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

### Δείτε επίσης

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


