---
title: "SaveOptions.PresentationFormat"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает PresentationFormat, в котором будет сохранён документ."
type: docs
weight: 140
url: /ru/net/aspose.tasks.saving/saveoptions/presentationformat/
---
## SaveOptions.PresentationFormat property

Получает или задает `PresentationFormat`, в котором будет сохранён документ.

```csharp
public PresentationFormat PresentationFormat { get; set; }
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

Показывает, как отобразить представление использования задач с настройками шкалы времени, определенными в настройках представления.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// Определите SaveOptions и укажите, что следует использовать настройки масштаба времени TaskUsageView.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### См. также

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


