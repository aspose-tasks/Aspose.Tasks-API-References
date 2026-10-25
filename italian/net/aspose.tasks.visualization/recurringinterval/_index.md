---
title: "Classe RecurringInterval"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Visualization.RecurringInterval. Rappresenta gli intervalli ricorrenti utilizzati nelle linee di avanzamento di una vista Gantt Chart"
type: docs
weight: 3310
url: /it/net/aspose.tasks.visualization/recurringinterval/
---
## RecurringInterval class

Rappresenta gli intervalli ricorrenti usati nelle linee di avanzamento di una visualizzazione del diagramma di Gantt.

```csharp
public class RecurringInterval
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RecurringInterval](recurringinterval/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DailyDayNumber](../../aspose.tasks.visualization/recurringinterval/dailydaynumber/) { get; set; } | Ottiene o imposta il numero giornaliero del giorno. |
| [DailyWorkday](../../aspose.tasks.visualization/recurringinterval/dailyworkday/) { get; set; } | Ottiene o imposta un valore che indica se un giorno è lavorativo per le linee di avanzamento giornaliere. |
| [Interval](../../aspose.tasks.visualization/recurringinterval/interval/) { get; set; } | Ottiene o imposta l'intervallo ricorrente. Può essere qualsiasi valore del tipo [`Interval`](./interval/). |
| [MonthlyDay](../../aspose.tasks.visualization/recurringinterval/monthlyday/) { get; set; } | Ottiene o imposta un valore che indica se mostrare le linee di avanzamento mensili per giorno. |
| [MonthlyDayDayNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaydaynumber/) { get; set; } | Ottiene o imposta il numero del giorno delle linee di avanzamento mensili. |
| [MonthlyDayMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/) { get; set; } | Ottiene o imposta il numero del mese delle linee di avanzamento mensili. |
| [MonthlyFirstLast](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlast/) { get; set; } | Ottiene o imposta un valore che indica se mostrare le linee di avanzamento per il primo o l'ultimo giorno predefinito. |
| [MonthlyFirstLastDay](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastday/) { get; set; } | Ottiene o imposta il tipo di giorno primo o ultimo delle linee di avanzamento mensili. |
| [MonthlyFirstLastMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastmonthnumber/) { get; set; } | Ottiene o imposta il numero del mese delle linee di avanzamento, che sono mostrate per il primo o l'ultimo giorno predefinito. |
| [WeeklyDays](../../aspose.tasks.visualization/recurringinterval/weeklydays/) { get; } | Ottiene un elenco di giorni per le linee di avanzamento settimanali. |
| [WeeklyWeekNumber](../../aspose.tasks.visualization/recurringinterval/weeklyweeknumber/) { get; set; } | Ottiene o imposta il numero della settimana per le linee di avanzamento settimanali. |

## Esempi

Mostra come lavorare con l'intervallo ricorrente delle linee di avanzamento.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

// consente di leggere la linea di avanzamento
var interval = view.ProgressLines.RecurringInterval;

Console.WriteLine("Interval: " + interval.Interval);
Console.WriteLine("Weekly Week Number: " + interval.WeeklyWeekNumber);
foreach (var day in interval.WeeklyDays)
{
    Console.WriteLine("Week day: " + day);
}

// consente di ridefinire l'intervallo ricorrente
var newInterval = new RecurringInterval();

// imposta un valore che indica se visualizzare le linee di avanzamento mensili per giorno.
interval.MonthlyDay = true;
// imposta il numero del giorno delle linee di avanzamento mensili.
interval.MonthlyDayDayNumber = 1;
// imposta il numero del mese delle linee di avanzamento mensili.
interval.MonthlyDayMonthNumber = 1;
// imposta un valore che indica se visualizzare le linee di avanzamento per il primo o l'ultimo giorno predefinito.
interval.MonthlyFirstLast = true;
// imposta il tipo di giorno (primo o ultimo) delle linee di avanzamento mensili.
interval.MonthlyFirstLastDay = RecurringInterval.DayType.Day;
// imposta il numero del mese delle linee di avanzamento, che sono visualizzate per il primo o l'ultimo giorno predefinito.
interval.MonthlyFirstLastMonthNumber = 1;

view.ProgressLines.RecurringInterval = newInterval;

project.Save(OutDir + "WorkWithRecurringInterval_out.pdf", SaveFileFormat.Pdf);
```

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


