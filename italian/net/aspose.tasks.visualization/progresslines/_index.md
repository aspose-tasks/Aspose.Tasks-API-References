---
title: "Classe ProgressLines"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Visualization.ProgressLines. Rappresenta le linee di avanzamento in una visualizzazione del diagramma di Gantt"
type: docs
weight: 3290
url: /it/net/aspose.tasks.visualization/progresslines/
---
## ProgressLines class

Rappresenta le linee di avanzamento in una visualizzazione del diagramma di Gantt.

```csharp
public class ProgressLines
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ProgressLines](progresslines/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BeginAtDate](../../aspose.tasks.visualization/progresslines/beginatdate/) { get; set; } | Ottiene o imposta la data da cui visualizzare le linee di avanzamento. |
| [BeginAtProjectStart](../../aspose.tasks.visualization/progresslines/beginatprojectstart/) { get; set; } | Ottiene o imposta un valore che indica se visualizzare le linee di avanzamento dall'inizio della data di avvio del progetto. |
| [DateFormat](../../aspose.tasks.visualization/progresslines/dateformat/) { get; set; } | Ottiene o imposta il formato della data ([`DateLabel`](../datelabel/)). |
| [DisplayAtCurrentDate](../../aspose.tasks.visualization/progresslines/displayatcurrentdate/) { get; set; } | Ottiene o imposta un valore che indica se visualizzare la linea di avanzamento alla data corrente. |
| [DisplayAtRecurringIntervals](../../aspose.tasks.visualization/progresslines/displayatrecurringintervals/) { get; set; } | Ottiene o imposta un valore che indica se visualizzare la linea di avanzamento a intervalli ricorrenti. |
| [DisplaySelected](../../aspose.tasks.visualization/progresslines/displayselected/) { get; set; } | Ottiene o imposta un valore che indica se visualizzare le linee di avanzamento alle date selezionate. |
| [Font](../../aspose.tasks.visualization/progresslines/font/) { get; set; } | Ottiene o imposta il carattere utilizzato per l'etichetta della linea di avanzamento. |
| [IsBaselinePlan](../../aspose.tasks.visualization/progresslines/isbaselineplan/) { get; set; } | Ottiene o imposta un valore che indica se visualizzare le linee di avanzamento per il piano di base o quello reale. |
| [LineColor](../../aspose.tasks.visualization/progresslines/linecolor/) { get; set; } | Ottiene o imposta il colore della linea per la linea di avanzamento corrente. |
| [LinePattern](../../aspose.tasks.visualization/progresslines/linepattern/) { get; set; } | Ottiene o imposta il modello di linea della linea di avanzamento corrente. [`LinePattern`](./linepattern/). |
| [OtherLineColor](../../aspose.tasks.visualization/progresslines/otherlinecolor/) { get; set; } | Ottiene o imposta il colore di un'altra linea di avanzamento. |
| [OtherLinePattern](../../aspose.tasks.visualization/progresslines/otherlinepattern/) { get; set; } | Ottiene o imposta il modello di linea per un'altra linea di avanzamento. |
| [OtherProgressPointColor](../../aspose.tasks.visualization/progresslines/otherprogresspointcolor/) { get; set; } | Ottiene o imposta il colore di un altro punto di avanzamento. |
| [OtherProgressPointShape](../../aspose.tasks.visualization/progresslines/otherprogresspointshape/) { get; set; } | Ottiene o imposta la forma del punto di avanzamento di un'altra linea di avanzamento. |
| [ProgressPointColor](../../aspose.tasks.visualization/progresslines/progresspointcolor/) { get; set; } | Ottiene o imposta il colore del punto di avanzamento. |
| [ProgressPointShape](../../aspose.tasks.visualization/progresslines/progresspointshape/) { get; set; } | Ottiene o imposta la forma del punto di avanzamento. [`GanttBarEndShape`](../ganttbarendshape/). |
| [RecurringInterval](../../aspose.tasks.visualization/progresslines/recurringinterval/) { get; set; } | Ottiene o imposta l'intervallo ricorrente. [`RecurringInterval`](./recurringinterval/). |
| [SelectedDates](../../aspose.tasks.visualization/progresslines/selecteddates/) { get; } | Ottiene l'elenco delle date selezionate per visualizzare le linee di avanzamento. |
| [ShowDate](../../aspose.tasks.visualization/progresslines/showdate/) { get; set; } | Ottiene o imposta un valore che indica se mostrare la data per ogni linea di avanzamento. |

## Esempi

Mostra come lavorare con le linee di avanzamento.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// definiamo la linea di avanzamento
view.ProgressLines = new ProgressLines();
var progressLines = view.ProgressLines;

// imposta la data da cui visualizzare le linee di avanzamento. Impostiamo la data di stato del progetto.
progressLines.BeginAtDate = project.Get(Prj.StatusDate);
// imposta un valore che indica se visualizzare le linee di avanzamento dall'inizio della data di avvio del progetto
progressLines.BeginAtProjectStart = true;
// imposta il formato della data (<see cref="T:Aspose.Tasks.Visualization.DateLabel" />).
progressLines.DateFormat = DateLabel.DayDddd;
// imposta un valore che indica se visualizzare la linea di avanzamento alla data corrente.
progressLines.DisplayAtCurrentDate = true;
// imposta un valore che indica se visualizzare la linea di avanzamento a intervalli ricorrenti.
progressLines.DisplayAtRecurringIntervals = true;
// imposta un valore che indica se visualizzare le linee di avanzamento alle date selezionate
progressLines.DisplaySelected = true;
// imposta un valore che indica se visualizzare le linee di avanzamento per il piano di base o reale.
progressLines.IsBaselinePlan = false;
// imposta il carattere utilizzato per l'etichetta della linea di avanzamento.
progressLines.Font = new FontDescriptor("Arial", 10);
// imposta il colore della linea per la linea di avanzamento corrente.
progressLines.LineColor = Color.Aquamarine;
// imposta il modello di linea della linea di avanzamento corrente.
progressLines.LinePattern = LinePattern.Dashed;
// imposta il colore dell'altra linea di avanzamento.
progressLines.OtherLineColor = Color.Azure;
// imposta il modello di linea per l'altra linea di avanzamento.
progressLines.OtherLinePattern = LinePattern.Dotted;
// imposta il colore dell'altro punto di avanzamento.
progressLines.OtherProgressPointColor = Color.Red;
// imposta la forma del punto di avanzamento dell'altra linea.
progressLines.OtherProgressPointShape = GanttBarEndShape.Circle;
// imposta il colore del punto di avanzamento.
progressLines.ProgressPointColor = Color.Orange;
// imposta la forma del punto di avanzamento.
progressLines.ProgressPointShape = GanttBarEndShape.Diamond;
// imposta l'intervallo ricorrente.
progressLines.RecurringInterval = new RecurringInterval();
// imposta l'intervallo ricorrente.
progressLines.RecurringInterval.Interval = Interval.Daily;
// imposta il numero giornaliero del giorno
progressLines.RecurringInterval.DailyDayNumber = 1;
// imposta un valore che indica se mostrare la data per ogni linea di avanzamento.
progressLines.ShowDate = true;

// verifichiamo le linee di avanzamento
Console.WriteLine("Begin At Date: " + progressLines.BeginAtDate);
Console.WriteLine("Begin At Project Start: " + progressLines.BeginAtProjectStart);
Console.WriteLine("Date Format: " + progressLines.DateFormat);
Console.WriteLine("Display At Current Date: " + progressLines.DisplayAtCurrentDate);
Console.WriteLine("Display At Recurring Intervals: " + progressLines.DisplayAtRecurringIntervals);
Console.WriteLine("Display Selected: " + progressLines.DisplaySelected);
Console.WriteLine("Font: " + progressLines.Font);
Console.WriteLine("Is Baseline Plan: " + progressLines.IsBaselinePlan);
Console.WriteLine("Line Color: " + progressLines.LineColor);
Console.WriteLine("Line Pattern: " + progressLines.LinePattern);
Console.WriteLine("Other Line Color: " + progressLines.OtherLineColor);
Console.WriteLine("Other Line Pattern: " + progressLines.OtherLinePattern);
Console.WriteLine("Other Progress Point Color: " + progressLines.OtherProgressPointColor);
Console.WriteLine("Other Progress Point Shape: " + progressLines.OtherProgressPointShape);
Console.WriteLine("Progress Point Color: " + progressLines.ProgressPointColor);
Console.WriteLine("Progress Point Shape: " + progressLines.ProgressPointShape);
Console.WriteLine("Recurring Interval: " + progressLines.RecurringInterval.Interval);
Console.WriteLine("Recurring Interval DailyDayNumber: " + progressLines.RecurringInterval.DailyDayNumber);
Console.WriteLine("Selected Dates: ");
foreach (var date in progressLines.SelectedDates)
{
    Console.WriteLine("Date: " + date);
}
Console.WriteLine("Show Date: " + progressLines.ShowDate);
Console.WriteLine();

project.Save(OutDir + "WorkWithProgressLines_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


