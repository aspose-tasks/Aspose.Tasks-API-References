---
title: SaveOptions.Gridlines
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets a list of Gridline that appear in project view
type: docs
weight: 60
url: /net/aspose.tasks.saving/saveoptions/gridlines/
---
## SaveOptions.Gridlines property

Gets or sets a list of [`Gridline`](../../../aspose.tasks.visualization/gridline/) that appear in project view.

```csharp
public List<Gridline> Gridlines { get; set; }
```

## Examples

Shows how to save layout to separate files.

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

// Save project layout to separate files
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### See Also

* class [Gridline](../../../aspose.tasks.visualization/gridline/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


