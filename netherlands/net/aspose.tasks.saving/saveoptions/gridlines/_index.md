---
title: "SaveOptions.Gridlines"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions eigenschap. Haalt een lijst van Gridline op of stelt deze in die verschijnen in de projectweergave"
type: docs
weight: 60
url: /nl/net/aspose.tasks.saving/saveoptions/gridlines/
---
## SaveOptions.Gridlines property

Haalt een lijst van [`Gridline`](../../../aspose.tasks.visualization/gridline/) op of stelt deze in die verschijnen in de projectweergave.

```csharp
public List<Gridline> Gridlines { get; set; }
```

## Voorbeelden

Toont hoe de lay‑out op te slaan in afzonderlijke bestanden.

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

// Projectlay-out opslaan in afzonderlijke bestanden
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### Zie ook

* class [Gridline](../../../aspose.tasks.visualization/gridline/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


