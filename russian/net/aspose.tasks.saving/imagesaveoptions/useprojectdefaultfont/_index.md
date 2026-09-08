---
title: "UseProjectDefaultFont"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Получает или задает значение, указывающее, должен ли использоваться шрифт по умолчанию для рендеринга."
type: docs
weight: 110
url: /ru/net/aspose.tasks.saving/imagesaveoptions/useprojectdefaultfont/
---
## ImageSaveOptions.UseProjectDefaultFont property

Получает или задает значение, указывающее, должен ли использоваться шрифт по умолчанию для рендеринга.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

### Примечания

Если значение равно False и указано DefaultFontName, движок рендеринга будет использовать шрифт, указанный в DefaultFontName, в качестве резервного шрифта. В противном случае в качестве резервного шрифта используются 'Arial' (если установлен) или шрифты 'Generic Sans Serif'. Резервный шрифт используется при рендеринге представления проекта, когда стиль текста ссылается на шрифт, не установленный в текущей операционной системе. Для более тонкого управления разрешением шрифтов вы можете использовать обратный вызов [`FontResolveCallback`](../fontresolvecallback).

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
