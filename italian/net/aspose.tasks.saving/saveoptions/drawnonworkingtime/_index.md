---
title: "SaveOptions.DrawNonWorkingTime"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta un valore che indica se il tempo non lavorativo deve essere disegnato. Il valore predefinito è TRUE."
type: docs
weight: 30
url: /it/net/aspose.tasks.saving/saveoptions/drawnonworkingtime/
---
## SaveOptions.DrawNonWorkingTime property

Ottiene o imposta un valore che indica se il tempo non lavorativo deve essere disegnato (Il valore predefinito è TRUE).

```csharp
public bool DrawNonWorkingTime { get; set; }
```

## Esempi

Mostra come impostare un valore che indica che le sottoattività sulla barra dell'attività di riepilogo devono essere aggregate.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // OPPURE
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### Vedi anche

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


