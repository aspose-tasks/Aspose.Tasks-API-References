---
title: "UseProjectDefaultFont"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η προεπιλεγμένη γραμματοσειρά πρέπει να χρησιμοποιείται για την απόδοση."
type: docs
weight: 180
url: /el/net/aspose.tasks.saving/htmlsaveoptions/useprojectdefaultfont/
---
## HtmlSaveOptions.UseProjectDefaultFont property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η προεπιλεγμένη γραμματοσειρά πρέπει να χρησιμοποιείται για την απόδοση.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

### Παρατηρήσεις

Όταν η τιμή είναι False και έχει οριστεί το DefaultFontName, η μηχανή απόδοσης θα χρησιμοποιήσει τη γραμματοσειρά που καθορίζεται από το DefaultFontName ως εφεδρική γραμματοσειρά. Διαφορετικά, χρησιμοποιούνται οι γραμματοσειρές 'Arial' (εάν είναι εγκατεστημένη) ή 'Generic Sans Serif' ως εφεδρική γραμματοσειρά. Η εφεδρική γραμματοσειρά χρησιμοποιείται κατά την απόδοση της προβολής του έργου όταν ένα στυλ κειμένου αναφέρεται σε γραμματοσειρά που δεν είναι εγκατεστημένη στο τρέχον λειτουργικό σύστημα. Για μεγαλύτερο έλεγχο της ανάλυσης γραμματοσειρών, μπορείτε να χρησιμοποιήσετε το callback [`FontResolveCallback`](../fontresolvecallback).

### Παραδείγματα

Δείχνει πώς να ορίσετε προσαρμοσμένη γραμματοσειρά που θα χρησιμοποιηθεί για την εξαγωγή του έργου σε αρχείο HTML.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true,
                      UseProjectDefaultFont = false,
                      DefaultFontName = "Segoe UI Black"
                  };
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### Δείτε επίσης

* class [HtmlSaveOptions](../../htmlsaveoptions)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- ΜΗ ΕΠΕΞΕΡΓΑΣΙΑ: δημιουργήθηκε από xmldocmd για Aspose.Tasks.dll -->
