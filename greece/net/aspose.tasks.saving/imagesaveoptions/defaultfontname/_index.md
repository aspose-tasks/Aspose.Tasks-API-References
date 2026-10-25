---
title: "DefaultFontName"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Λαμβάνει ή ορίζει τη προεπιλεγμένη ή εφεδρική font για την απόδοση."
type: docs
weight: 20
url: /el/net/aspose.tasks.saving/imagesaveoptions/defaultfontname/
---
## ImageSaveOptions.DefaultFontName property

Λαμβάνει ή ορίζει την προεπιλεγμένη (ή εφεδρική) γραμματοσειρά για την απόδοση.

```csharp
public string DefaultFontName { get; set; }
```

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
