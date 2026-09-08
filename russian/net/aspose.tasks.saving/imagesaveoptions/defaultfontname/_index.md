---
title: "DefaultFontName"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Получает или задает шрифт по умолчанию или резервный шрифт для рендеринга."
type: docs
weight: 20
url: /ru/net/aspose.tasks.saving/imagesaveoptions/defaultfontname/
---
## ImageSaveOptions.DefaultFontName property

Получает или задает шрифт по умолчанию (или резервный) для рендеринга.

```csharp
public string DefaultFontName { get; set; }
```

### Примеры

Показывает, как сохранить макет в отдельные файлы.

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

// Сохранить макет проекта в отдельные файлы
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### См. также

* class [ImageSaveOptions](../../imagesaveoptions)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для Aspose.Tasks.dll -->
