---
title: "PageViewSettings.PrintAllSheetColumns"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PageViewSettings. Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν θα εκτυπωθούν όλες οι στήλες φύλλου μιας προβολής"
type: docs
weight: 40
url: /el/net/aspose.tasks.visualization/pageviewsettings/printallsheetcolumns/
---
## PageViewSettings.PrintAllSheetColumns property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εκτυπωθούν όλες οι στήλες φύλλου μιας προβολής.

```csharp
public bool PrintAllSheetColumns { get; set; }
```

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

* class [PageViewSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pageviewsettings/)
* assembly [Aspose.Tasks](../../../)


