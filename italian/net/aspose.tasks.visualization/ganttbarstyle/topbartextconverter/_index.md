---
title: "GanttBarStyle.TopBarTextConverter"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà GanttBarStyle. Ottiene o imposta il convertitore definito dall'utente per ottenere il testo da visualizzare in alto sulla barra delle attività. Sovrascrive il valore della proprietà TopField"
type: docs
weight: 260
url: /it/net/aspose.tasks.visualization/ganttbarstyle/topbartextconverter/
---
## GanttBarStyle.TopBarTextConverter property

Ottiene o imposta il convertitore definito dall'utente per ottenere il testo da visualizzare in alto sulla barra dell'attività. Sovrascrive il valore della proprietà [`TopField`](../topfield/).

```csharp
public TaskBarTextConverter TopBarTextConverter { get; set; }
```

## Osservazioni

Non viene salvato nel formato MPP.

## Esempi

Mostra come utilizzare gli stili di barra personalizzati della vista del diagramma di Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// Gli stili di barra possono essere specifici per attività (situati in GanttChartView.CustomBarStyles)
// o specifici per categoria (situati in GanttChartView.BarStyles)
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // Per scopi dimostrativi stiamo modificando lo stile per l'attività con ID univoco = 4
    // Qui impostiamo il campo (TaskName) per renderlo a sinistra della barra dell'attività.
    ganttBarStyle.LeftField = Field.TaskName;
    // Qui impostiamo un convertitore personalizzato per controllare quale testo deve essere visualizzato all'interno della barra dell'attività.
    ganttBarStyle.InsideBarTextConverter = task => "Hours rem.: " + (int)task.Get(Tsk.RemainingWork).TimeSpan.TotalHours;

    ganttBarStyle.MiddleShapeColor = Color.Green;
    ganttBarStyle.MiddleShape = GanttBarMiddleShape.LineTop;
    ganttBarStyle.StartShape = GanttBarEndShape.LeftBracket;
    ganttBarStyle.StartShapeColor = Color.Aqua;
    ganttBarStyle.EndShape = GanttBarEndShape.RightBracket;
    ganttBarStyle.EndShapeColor = Color.Aquamarine;
}

foreach (GanttBarStyle ganttBarStyle in ganttChartView.BarStyles)
{
    if (!ganttBarStyle.ShowForCategories.Contains(GanttBarShowFor.Milestone))
    {
        continue;
    }

    // Per scopi dimostrativi stiamo modificando gli stili applicabili alle attività milestone.

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

### Vedi anche

* delegate [TaskBarTextConverter](../../taskbartextconverter/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


