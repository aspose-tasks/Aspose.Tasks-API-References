---
title: "SaveOptions.StartDate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει την ημερομηνία από την οποία θα ξεκινήσει η απόδοση."
type: docs
weight: 170
url: /el/net/aspose.tasks.saving/saveoptions/startdate/
---
## SaveOptions.StartDate property

Λαμβάνει ή ορίζει την ημερομηνία από την οποία θα ξεκινήσει η απόδοση.

```csharp
public DateTime StartDate { get; set; }
```

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε τη διάταξη σε ξεχωριστά αρχεία.

```csharp
var project = new Project(DataDir + "Homemoveplan.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);
options.StartDate = project.Get(Prj.StartDate).AddDays(-3);
options.EndDate = project.Get(Prj.FinishDate);
options.MarkCriticalTasks = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.FontSettings.DefaultFontName = "Segoe UI Black";
options.FontSettings.UseProjectDefaultFont = false;
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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


