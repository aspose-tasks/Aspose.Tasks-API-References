---
title: "Κλάση PageViewSettings"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.PageViewSettings class. Αντιπροσωπεύει τις ρυθμίσεις εκτύπωσης για μια προβολή έργου"
type: docs
weight: 3260
url: /el/net/aspose.tasks.visualization/pageviewsettings/
---
## PageViewSettings class

Αναπαριστά τις ρυθμίσεις εκτύπωσης για μια προβολή του έργου.

```csharp
public class PageViewSettings
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PageViewSettings](pageviewsettings/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [FirstColumnsCount](../../aspose.tasks.visualization/pageviewsettings/firstcolumnscount/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό των πρώτων στηλών που θα εκτυπωθούν σε όλες τις σελίδες. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.visualization/pageviewsettings/fittimescaletoendofpage/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα προσαρμοστεί η κλίμακα χρόνου στο τέλος μιας σελίδας κατά την εκτύπωση. |
| [PrintAllSheetColumns](../../aspose.tasks.visualization/pageviewsettings/printallsheetcolumns/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εκτυπωθούν όλες οι στήλες φύλλου μιας προβολής. |
| [PrintBlankPages](../../aspose.tasks.visualization/pageviewsettings/printblankpages/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εκτυπωθούν κενές σελίδες μιας προβολής. |
| [PrintFirstColumnsCountOnAllPages](../../aspose.tasks.visualization/pageviewsettings/printfirstcolumnscountonallpages/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εκτυπωθεί καθορισμένος αριθμός των πρώτων στηλών σε όλες τις σελίδες. |
| [PrintNotes](../../aspose.tasks.visualization/pageviewsettings/printnotes/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εκτυπωθούν σημειώσεις. |

## Παραδείγματα

Δείχνει πώς να εκτυπώσετε σημειώσεις εργασιών, πόρων και εκχωρήσεων σε ξεχωριστή σελίδα.

```csharp
var project = new Project(DataDir + "Input.mpp");

// ορίστε τον αριθμό των πρώτων στηλών που θα εκτυπωθούν σε όλες τις σελίδες
project.DefaultView.PageInfo.PageViewSettings.FirstColumnsCount = 2;

// ορίστε μια τιμή που υποδεικνύει εάν θα εκτυπωθούν σημειώσεις.
project.DefaultView.PageInfo.PageViewSettings.PrintNotes = true;

// ορίστε μια τιμή που υποδεικνύει εάν θα προσαρμοστεί η κλίμακα χρόνου στο τέλος μιας σελίδας κατά την εκτύπωση.
project.DefaultView.PageInfo.PageViewSettings.FitTimescaleToEndOfPage = true;

// ορίστε μια τιμή που υποδεικνύει εάν θα εκτυπωθούν όλες οι στήλες φύλλου μιας προβολής
project.DefaultView.PageInfo.PageViewSettings.PrintAllSheetColumns = true;

// ορίστε μια τιμή που υποδεικνύει εάν θα εκτυπωθούν κενές σελίδες μιας προβολής
project.DefaultView.PageInfo.PageViewSettings.PrintBlankPages = false;

// ορίστε μια τιμή που υποδεικνύει εάν θα εκτυπωθεί καθορισμένος αριθμός πρώτων στηλών σε όλες τις σελίδες
project.DefaultView.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

project.Save(OutDir + "ProjectWithComments_out.pdf", SaveFileFormat.Pdf);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


