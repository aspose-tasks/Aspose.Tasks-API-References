---
title: "DefaultFontName"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Λαμβάνει ή ορίζει τη προεπιλεγμένη ή εφεδρική font για την απόδοση."
type: docs
weight: 40
url: /el/net/aspose.tasks.saving/htmlsaveoptions/defaultfontname/
---
## HtmlSaveOptions.DefaultFontName property

Λαμβάνει ή ορίζει την προεπιλεγμένη (ή εφεδρική) γραμματοσειρά για την απόδοση.

```csharp
public string DefaultFontName { get; set; }
```

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
