---
title: SaveOptions.StartDate
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets the date to start rendering from
type: docs
weight: 170
url: /net/aspose.tasks.saving/saveoptions/startdate/
---
## SaveOptions.StartDate property

Gets or sets the date to start rendering from.

```csharp
public DateTime StartDate { get; set; }
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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


