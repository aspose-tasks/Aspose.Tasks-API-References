---
title: "RecurringInterval.DailyWorkday"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "RecurringInterval proprietà. Ottiene o imposta un valore che indica se un giorno è lavorativo per le linee di avanzamento giornaliere"
type: docs
weight: 30
url: /it/net/aspose.tasks.visualization/recurringinterval/dailyworkday/
---
## RecurringInterval.DailyWorkday property

Ottiene o imposta un valore che indica se un giorno è lavorativo per le linee di avanzamento giornaliere.

```csharp
public bool DailyWorkday { get; set; }
```

## Esempi

Mostra come aggiungere un intervallo ricorrente giornaliero di linee di avanzamento.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

view.ProgressLines.RecurringInterval = new RecurringInterval();
// imposta il numero del giorno del modello giornaliero
view.ProgressLines.RecurringInterval.DailyDayNumber = 2;
// imposta un valore che indica se un giorno è lavorativo per le linee di avanzamento giornaliere.
view.ProgressLines.RecurringInterval.DailyWorkday = true;
```

### Vedi anche

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


