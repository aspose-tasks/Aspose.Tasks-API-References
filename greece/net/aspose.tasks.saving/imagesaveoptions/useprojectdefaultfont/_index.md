---
title: "UseProjectDefaultFont"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η προεπιλεγμένη γραμματοσειρά πρέπει να χρησιμοποιείται για την απόδοση."
type: docs
weight: 110
url: /el/net/aspose.tasks.saving/imagesaveoptions/useprojectdefaultfont/
---
## ImageSaveOptions.UseProjectDefaultFont property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η προεπιλεγμένη γραμματοσειρά πρέπει να χρησιμοποιείται για την απόδοση.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

### Παρατηρήσεις

Όταν η τιμή είναι False και έχει οριστεί το DefaultFontName, η μηχανή απόδοσης θα χρησιμοποιήσει τη γραμματοσειρά που καθορίζεται από το DefaultFontName ως εφεδρική γραμματοσειρά. Διαφορετικά, χρησιμοποιούνται οι γραμματοσειρές 'Arial' (εάν είναι εγκατεστημένη) ή 'Generic Sans Serif' ως εφεδρική γραμματοσειρά. Η εφεδρική γραμματοσειρά χρησιμοποιείται κατά την απόδοση της προβολής του έργου όταν ένα στυλ κειμένου αναφέρεται σε γραμματοσειρά που δεν είναι εγκατεστημένη στο τρέχον λειτουργικό σύστημα. Για μεγαλύτερο έλεγχο της ανάλυσης γραμματοσειρών, μπορείτε να χρησιμοποιήσετε το callback [`FontResolveCallback`](../fontresolvecallback).

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε τη διάταξη σε ξεχωριστά αρχεία.

```csharp
var project = new Project(DataDir + "Homemoveplan.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);
options.StartDate = project.Get(Prj.StartDate).AddDays(-3);
options.EndDate = project.Get(Prj.FinishDate);
options.MarkCriticalTasks = true;
options.DefaultFontName = "Segoe UI Black";
options.UseProjectDefaultFont = false;
options.PageSize = PageSize.Letter;

options.Gridlines = new List<Gridline>();

var gridline = new Gridline { GridlineType = GridlineType.GanttRow, Color = Color.CornflowerBlue, Pattern = LinePattern.Dashed };
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles1_out.png", options);

// Αποθήκευση διάταξης έργου σε ξεχωριστά αρχεία
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### Δείτε επίσης

* class [ImageSaveOptions](../../imagesaveoptions)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- ΜΗ ΕΠΕΞΕΡΓΑΣΙΑ: δημιουργήθηκε από xmldocmd για Aspose.Tasks.dll -->
