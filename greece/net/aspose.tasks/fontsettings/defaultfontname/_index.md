---
title: "FontSettings.DefaultFontName"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα FontSettings. Λαμβάνει ή ορίζει τη προεπιλεγμένη ή εναλλακτική γραμματοσειρά για απόδοση."
type: docs
weight: 20
url: /el/net/aspose.tasks/fontsettings/defaultfontname/
---
## FontSettings.DefaultFontName property

Λαμβάνει ή ορίζει την προεπιλεγμένη (ή εφεδρική) γραμματοσειρά για την απόδοση.

```csharp
public string DefaultFontName { get; set; }
```

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


