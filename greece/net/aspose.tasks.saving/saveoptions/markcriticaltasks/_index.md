---
title: "SaveOptions.MarkCriticalTasks"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν οι κρίσιμες εργασίες πρέπει να εμφανίζονται με κόκκινο χρώμα. Η προεπιλεγμένη τιμή είναι FALSE."
type: docs
weight: 100
url: /el/net/aspose.tasks.saving/saveoptions/markcriticaltasks/
---
## SaveOptions.MarkCriticalTasks property

Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν οι κρίσιμες εργασίες πρέπει να εμφανίζονται με κόκκινο χρώμα (Η προεπιλεγμένη τιμή είναι FALSE).

```csharp
public bool MarkCriticalTasks { get; set; }
```

## Παραδείγματα

Δείχνει πώς να εκτυπώσετε τις κρίσιμες εργασίες κατά την αποθήκευση σε μορφές αρχείων εικόνας.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png)
{
    StartDate = project.Get(Prj.StartDate).AddDays(-3),
    EndDate = project.Get(Prj.FinishDate),
    MarkCriticalTasks = true,
    LegendDrawingOptions = LegendDrawingOptions.NoLegend,
    Gridlines = new List<Gridline>()
};

var gridline = new Gridline { GridlineType = GridlineType.GanttRow, Color = Color.CornflowerBlue, Pattern = LinePattern.Dashed };
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles1_out.png", options);

// Αποθήκευση διάταξης έργου σε ξεχωριστά αρχεία
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### Δείτε επίσης

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


