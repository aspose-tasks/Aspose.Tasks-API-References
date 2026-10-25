---
title: "GanttChartView.HideRollupBarsWhenSummaryExpanded"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà GanttChartView. Ottiene o imposta un valore che indica se le barre di riepilogo saranno nascoste durante l'espansione dell'attività di riepilogo"
type: docs
weight: 90
url: /it/net/aspose.tasks/ganttchartview/hiderollupbarswhensummaryexpanded/
---
## GanttChartView.HideRollupBarsWhenSummaryExpanded property

Ottiene o imposta un valore che indica se le barre di riepilogo saranno nascoste durante l'espansione del task riepilogativo.

```csharp
public bool HideRollupBarsWhenSummaryExpanded { get; set; }
```

## Esempi

Mostra come impostare alcune proprietà utili della visualizzazione del diagramma di Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// imposta un valore che indica se le barre vengono arrotondate al giorno più vicino
view.BarRounding = false;
// imposta l'altezza, in punti, delle barre Gantt nel diagramma di Gantt
view.BarSize = GanttBarSize.BarSize24;
// imposta un valore che indica se le barre di riepilogo saranno nascoste durante l'espansione dell'attività di riepilogo
view.HideRollupBarsWhenSummaryExpanded = true;
// imposta il colore del tempo non lavorativo
view.NonWorkingTimeColor = Color.Azure;
// imposta un valore che indica se le barre nel diagramma di Gantt devono essere raggruppate
view.RollUpGanttBars = true;
// imposta un valore che indica se le divisioni delle attività nel diagramma di Gantt devono essere visualizzate
view.ShowBarSplits = true;
// imposta un valore che indica se i disegni nel diagramma di Gantt devono essere visualizzati
view.ShowDrawings = true;
// imposta una percentuale per ridurre o aumentare la spaziatura tra le unità nel livello della scala temporale
view.TimescaleSizePercentage = 10;

project.Save(OutDir + "WorkWithGanttChartViews_out.pdf", SaveFileFormat.Pdf);
```

### Vedi anche

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


