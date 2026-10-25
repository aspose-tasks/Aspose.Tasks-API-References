---
title: "Κλάση PageSettings"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Visualization.PageSettings. Αντιπροσωπεύει τις ρυθμίσεις εκτύπωσης για μια σελίδα της προβολής έργου"
type: docs
weight: 3240
url: /el/net/aspose.tasks.visualization/pagesettings/
---
## PageSettings class

Αναπαριστά τις ρυθμίσεις εκτύπωσης για μια σελίδα της προβολής του έργου.

```csharp
public class PageSettings
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PageSettings](pagesettings/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `PageSettings`. Αντιπροσωπεύει τις ρυθμίσεις εκτύπωσης για μια σελίδα της προβολής έργου. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AdjustToPercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα προσαρμόσει την εκτύπωση στο καθορισμένο ποσοστό ([`PercentOfNormalSize`](./percentofnormalsize/)) του κανονικού μεγέθους. |
| [FirstPageNumber](../../aspose.tasks.visualization/pagesettings/firstpagenumber/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό της πρώτης σελίδας για εκτύπωση. |
| [IsPortrait](../../aspose.tasks.visualization/pagesettings/isportrait/) { get; set; } | Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν ο προσανατολισμός της σελίδας είναι πορτραίτο· επιστρέφει false εάν ο προσανατολισμός της σελίδας είναι τοπίο. |
| [PagesInHeight](../../aspose.tasks.visualization/pagesettings/pagesinheight/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό των σελίδων σε ύψος που θα εκτυπωθούν. |
| [PagesInWidth](../../aspose.tasks.visualization/pagesettings/pagesinwidth/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό των σελίδων σε πλάτος που θα εκτυπωθούν. |
| [PaperSize](../../aspose.tasks.visualization/pagesettings/papersize/) { get; set; } | Λαμβάνει ή ορίζει το μέγεθος του χαρτιού. Μπορεί να είναι μία από τις τιμές της απαρίθμησης [`PrinterPaperSize`](../printerpapersize/). |
| [PaperSizeId](../../aspose.tasks.visualization/pagesettings/papersizeid/) { get; set; } | Λαμβάνει ή ορίζει έναν ακέραιο που αντιπροσωπεύει μία από τις τιμές του PrinterPaperSize ή ένα προσαρμοσμένο αναγνωριστικό μεγέθους σελίδας. Αυτή η τιμή μπορεί να χρησιμοποιηθεί για την ανάκτηση του PaperSize από τις ρυθμίσεις του λειτουργικού συστήματος. |
| [PercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/percentofnormalsize/) { get; set; } | Λαμβάνει ή ορίζει ένα ποσοστό του κανονικού μεγέθους για προσαρμογή της εκτύπωσης. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


