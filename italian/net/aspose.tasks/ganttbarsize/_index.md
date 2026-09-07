---
title: "Enum GanttBarSize"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.GanttBarSize. Specifica l'altezza di una barra in punti"
type: docs
weight: 700
url: /it/net/aspose.tasks/ganttbarsize/
---
## GanttBarSize enumeration

Specifica l'altezza di una barra in punti.

```csharp
public enum GanttBarSize
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| BarSize6 | `0` | Dimensione barra 6 punti. |
| BarSize8 | `1` | Dimensione barra 8 punti. |
| BarSize10 | `2` | Dimensione barra 10 punti. |
| BarSize12 | `3` | Dimensione barra 12 punti. |
| BarSize14 | `4` | Dimensione barra 14 punti. |
| BarSize18 | `5` | Dimensione barra 18 punti. |
| BarSize24 | `6` | Dimensione barra 24 punti. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


