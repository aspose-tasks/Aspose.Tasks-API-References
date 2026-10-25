---
title: "SaveOptions.Gridlines"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveOptions. Obtient ou définit une liste de Gridline qui apparaît dans la vue du projet"
type: docs
weight: 60
url: /fr/net/aspose.tasks.saving/saveoptions/gridlines/
---
## SaveOptions.Gridlines property

Obtient ou définit une liste de [`Gridline`](../../../aspose.tasks.visualization/gridline/) qui apparaît dans la vue du projet.

```csharp
public List<Gridline> Gridlines { get; set; }
```

## Exemples

Montre comment enregistrer la mise en page dans des fichiers séparés.

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

// Enregistrer la mise en page du projet dans des fichiers séparés
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### Voir aussi

* class [Gridline](../../../aspose.tasks.visualization/gridline/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


