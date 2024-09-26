---
title: SaveOptions.MarkCriticalTasks
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets a value indicating whether critical tasks should be displayed in red color Default value is FALSE
type: docs
weight: 100
url: /net/aspose.tasks.saving/saveoptions/markcriticaltasks/
---
## SaveOptions.MarkCriticalTasks property

Gets or sets a value indicating whether critical tasks should be displayed in red color (Default value is FALSE).

```csharp
public bool MarkCriticalTasks { get; set; }
```

## Examples

Shows how to print critical tasks while save in image file formats.

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

// Save project layout to separate files
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


