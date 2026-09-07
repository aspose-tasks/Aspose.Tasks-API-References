---
title: "DefaultFontName"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Λαμβάνει ή ορίζει τη προεπιλεγμένη ή εφεδρική font για την απόδοση."
type: docs
weight: 30
url: /el/net/aspose.tasks.saving/pdfsaveoptions/defaultfontname/
---
## PdfSaveOptions.DefaultFontName property

Λαμβάνει ή ορίζει την προεπιλεγμένη (ή εφεδρική) γραμματοσειρά για την απόδοση.

```csharp
public string DefaultFontName { get; set; }
```

### Παραδείγματα

Δείχνει πώς να ορίσετε προσαρμοσμένη γραμματοσειρά που θα χρησιμοποιηθεί για την εκτύπωση του τελικού PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true, UseProjectDefaultFont = false, DefaultFontName = "Segoe UI Black"
                  };
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### Δείτε επίσης

* class [PdfSaveOptions](../../pdfsaveoptions)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- ΜΗ ΕΠΕΞΕΡΓΑΣΙΑ: δημιουργήθηκε από xmldocmd για Aspose.Tasks.dll -->
