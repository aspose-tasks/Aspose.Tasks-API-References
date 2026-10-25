---
title: "SaveOptions.RollUpGanttBars"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta un valore che indica se le sottoattività sulla barra dell'attività riepilogo devono essere contrassegnate. Per le sottoattività, il campo Rollup indica se le informazioni sulle barre Gantt delle sottoattività saranno aggregate nella barra dell'attività riepilogo. Per le attività riepilogo, il campo Rollup indica se la barra dell'attività riepilogo visualizza barre aggregate. È necessario impostare il campo Rollup per le attività riepilogo su Sì affinché le sottoattività vengano aggregate."
type: docs
weight: 160
url: /it/net/aspose.tasks.saving/saveoptions/rollupganttbars/
---
## SaveOptions.RollUpGanttBars property

Ottiene o imposta un valore che indica se le sottoattività sulla barra dell'attività di riepilogo devono essere contrassegnate. Per le sottoattività, il campo Rollup indica se le informazioni sulle barre Gantt delle sottoattività verranno aggregate nella barra dell'attività di riepilogo. Per le attività di riepilogo, il campo Rollup indica se la barra dell'attività di riepilogo visualizza le barre aggregate. È necessario impostare il campo Rollup per le attività di riepilogo su Yes affinché le sottoattività vengano aggregate.

```csharp
public bool RollUpGanttBars { get; set; }
```

## Osservazioni

È applicabile solo quando la vista del diagramma di Gantt viene renderizzata.

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


