---
title: "RecurringInterval.WeeklyDays"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà RecurringInterval. Ottiene un elenco di giorni per le linee di avanzamento settimanali"
type: docs
weight: 110
url: /it/net/aspose.tasks.visualization/recurringinterval/weeklydays/
---
## RecurringInterval.WeeklyDays property

Ottiene un elenco di giorni per le linee di avanzamento settimanali.

```csharp
public List<DayType> WeeklyDays { get; }
```

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

* enum [DayType](../../recurringinterval.daytype/)
* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


