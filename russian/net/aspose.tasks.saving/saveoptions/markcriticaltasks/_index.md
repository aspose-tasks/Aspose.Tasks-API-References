---
title: "SaveOptions.MarkCriticalTasks"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает значение, указывающее, должны ли критические задачи отображаться красным цветом. Значение по умолчанию – FALSE."
type: docs
weight: 100
url: /ru/net/aspose.tasks.saving/saveoptions/markcriticaltasks/
---
## SaveOptions.MarkCriticalTasks property

Получает или задает значение, указывающее, должны ли критические задачи отображаться красным цветом (значение по умолчанию — FALSE).

```csharp
public bool MarkCriticalTasks { get; set; }
```

## Примеры

Показано, как выводить критические задачи при сохранении в форматы файлов изображений.

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

// Сохранить макет проекта в отдельные файлы
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


