---
title: "FontSettings.UseProjectDefaultFont"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα FontSettings. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η προεπιλεγμένη γραμματοσειρά πρέπει να χρησιμοποιηθεί για απόδοση"
type: docs
weight: 40
url: /el/net/aspose.tasks/fontsettings/useprojectdefaultfont/
---
## FontSettings.UseProjectDefaultFont property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η προεπιλεγμένη γραμματοσειρά πρέπει να χρησιμοποιείται για την απόδοση.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

## Παρατηρήσεις

Όταν η τιμή είναι False και έχει καθοριστεί το DefaultFontName, η μηχανή απόδοσης θα χρησιμοποιήσει τη γραμματοσειρά που έχει οριστεί από το DefaultFontName ως εφεδρική γραμματοσειρά. Διαφορετικά, χρησιμοποιούνται οι γραμματοσειρές 'Arial' (αν είναι εγκατεστημένη) ή 'Generic Sans Serif' ως εφεδρική γραμματοσειρά. Η εφεδρική γραμματοσειρά χρησιμοποιείται κατά την απόδοση της προβολής έργου όταν ένα στυλ κειμένου αναφέρεται σε γραμματοσειρά που δεν είναι εγκατεστημένη στο τρέχον λειτουργικό σύστημα. Για μεγαλύτερο έλεγχο της επίλυσης γραμματοσειρών μπορείτε να χρησιμοποιήσετε το callback [`FontResolveCallback`](../fontresolvecallback/).

## Παραδείγματα

Δείχνει πώς να ορίσετε προσαρμοσμένη γραμματοσειρά που θα χρησιμοποιηθεί για την εκτύπωση του τελικού PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### Δείτε επίσης

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


