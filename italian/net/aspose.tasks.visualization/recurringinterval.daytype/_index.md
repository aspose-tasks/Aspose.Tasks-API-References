---
title: "Enum RecurringInterval.DayType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.RecurringIntervalDayType enum. Rappresenta un tipo di giorno usato nelle linee di avanzamento"
type: docs
weight: 3320
url: /it/net/aspose.tasks.visualization/recurringinterval.daytype/
---
## RecurringInterval.DayType enumeration

Rappresenta un tipo di giorno usato nelle linee di avanzamento.

```csharp
public enum DayType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Sunday | `1` | Indica domenica. |
| Monday | `2` | Indica lunedì. |
| Tuesday | `3` | Indica martedì. |
| Wednesday | `4` | Indica mercoledì. |
| Thursday | `5` | Indica giovedì. |
| Friday | `6` | Indica venerdì. |
| Saturday | `7` | Indica sabato. |
| Day | `8` | Indica giorno. |
| Workday | `9` | Indica giorno lavorativo. |
| NonworkingDay | `10` | Indica giorno non lavorativo. |

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

* class [RecurringInterval](../recurringinterval/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


