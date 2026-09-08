---
title: "SaveOptions.RenderToSinglePage"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает значение, указывающее, следует ли рендерить проект на одну страницу при сохранении проекта в графическом формате. Размер страницы будет изменён, чтобы отрендеренный проект поместился на одной странице."
type: docs
weight: 150
url: /ru/net/aspose.tasks.saving/saveoptions/rendertosinglepage/
---
## SaveOptions.RenderToSinglePage property

Получает или задает значение, указывающее, следует ли рендерить проект в одну страницу при сохранении проекта в графическом формате. Размер страницы будет изменён, чтобы отрисованный проект поместился на одной странице.

```csharp
public bool RenderToSinglePage { get; set; }
```

## Примеры

Показывает, как сохранить выбранные страницы проекта в PDF‑файл.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// проверим, сколько страниц можно экспортировать
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

Показывает, как использовать свойство RenderToSinglePage, чтобы указать, что проект должен быть сохранён в PDF на одну страницу.

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

Показывает, как сохранить выбранные страницы в виде изображения.

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

Показывает, как сохранить макет в отдельные файлы.

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

// Сохранить макет проекта в отдельные файлы
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


