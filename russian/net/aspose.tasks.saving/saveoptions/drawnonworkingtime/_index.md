---
title: "SaveOptions.DrawNonWorkingTime"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает значение, указывающее, следует ли отображать нерабочее время. Значение по умолчанию – TRUE."
type: docs
weight: 30
url: /ru/net/aspose.tasks.saving/saveoptions/drawnonworkingtime/
---
## SaveOptions.DrawNonWorkingTime property

Получает или задает значение, указывающее, следует ли отображать нерабочее время (значение по умолчанию — TRUE).

```csharp
public bool DrawNonWorkingTime { get; set; }
```

## Примеры

Показывает, как установить значение, указывающее, что подзадачи на полосе сводной задачи должны быть свернуты.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // ИЛИ
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


