---
title: "DefaultFontName"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Ottiene o imposta il font predefinito o di riserva per il rendering."
type: docs
weight: 20
url: /it/net/aspose.tasks.saving/imagesaveoptions/defaultfontname/
---
## ImageSaveOptions.DefaultFontName property

Ottiene o imposta il carattere predefinito (o di riserva) per il rendering.

```csharp
public string DefaultFontName { get; set; }
```

### Esempi

Mostra come salvare il layout in file separati.

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

// Salva il layout del progetto in file separati
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### Vedi anche

* class [ImageSaveOptions](../../imagesaveoptions)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per Aspose.Tasks.dll -->
