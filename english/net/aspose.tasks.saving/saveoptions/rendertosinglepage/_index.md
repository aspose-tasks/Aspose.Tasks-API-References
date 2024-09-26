---
title: SaveOptions.RenderToSinglePage
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets a value indicating whether a project should be rendered to a single page when project is saved in graphical format. The page size will be changed so the rendered project can be fit on one page
type: docs
weight: 150
url: /net/aspose.tasks.saving/saveoptions/rendertosinglepage/
---
## SaveOptions.RenderToSinglePage property

Gets or sets a value indicating whether a project should be rendered to a single page when project is saved in graphical format. The page size will be changed so the rendered project can be fit on one page.

```csharp
public bool RenderToSinglePage { get; set; }
```

## Examples

Shows how to save selected pages of a project into PDF file.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// lets check the number of pages can be exported
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

Shows how to use RenderToSinglePage property to specify that project should be saved to 1-page PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.TaskUsage;
options.Timescale = Timescale.DefinedInView;
options.RenderToSinglePage = true;
options.StartDate = new DateTime(2012, 12, 22);
options.EndDate = new DateTime(2013, 05, 10);

project.Save(OutDir + "WorkWithRenderToSinglePage_out.pdf", options);
```

Shows how to save selected pages in as an image.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

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


