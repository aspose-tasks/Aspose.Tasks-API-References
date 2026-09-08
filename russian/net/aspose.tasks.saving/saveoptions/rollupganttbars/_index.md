---
title: "SaveOptions.RollUpGanttBars"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает значение, указывающее, следует ли помечать подпункты на полосе задачи‑сводки. Для подпунктов поле Rollup указывает, будет ли информация о подпунктах Gantt‑полос свёрнута в полосу задачи‑сводки. Для задач‑сводок поле Rollup указывает, отображает ли полоса задачи‑сводки свёрнутые полосы. Вы должны установить поле Rollup для задач‑сводок в значение Yes, чтобы любые подпункты могли быть свёрнуты в них."
type: docs
weight: 160
url: /ru/net/aspose.tasks.saving/saveoptions/rollupganttbars/
---
## SaveOptions.RollUpGanttBars property

Получает или задает значение, указывающее, следует ли помечать подпроекты на полосе сводной задачи. Для подпроектов поле Rollup указывает, будет ли информация о ганттовых полосах подпроекта агрегирована в полосу сводной задачи. Для сводных задач поле Rollup указывает, отображает ли полоса сводной задачи агрегированные полосы. Для того чтобы любые подпроекты агрегировались, поле Rollup для сводных задач должно быть установлено в Yes.

```csharp
public bool RollUpGanttBars { get; set; }
```

## Примечания

Применяется только при рендеринге представления диаграммы Ганта.

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


