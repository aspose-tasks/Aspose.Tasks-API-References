---
title: "HtmlSaveOptions.UseGradientBrush"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα HtmlSaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί gradient brush κατά την απόδοση της διάταξης του έργου. Προς το παρόν η χρήση gradient brush δεν υποστηρίζεται κατά την απόδοση σε HTML"
type: docs
weight: 160
url: /el/net/aspose.tasks.saving/htmlsaveoptions/usegradientbrush/
---
## HtmlSaveOptions.UseGradientBrush property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί διαβαθμισμένο πινέλο κατά την απόδοση της διάταξης του έργου. Προς το παρόν η χρήση διαβαθμισμένου πινέλου δεν υποστηρίζεται κατά την απόδοση σε HTML.

```csharp
public override bool UseGradientBrush { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε προσαρμοσμένη γραμματοσειρά που θα χρησιμοποιηθεί για την εξαγωγή του έργου σε αρχείο HTML.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### Δείτε επίσης

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


