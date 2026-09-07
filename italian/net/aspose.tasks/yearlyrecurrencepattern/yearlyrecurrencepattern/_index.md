---
title: "YearlyRecurrencePattern.YearlyRecurrencePattern"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore YearlyRecurrencePattern. Inizializza una nuova istanza della classe YearlyRecurrencePattern"
type: docs
weight: 10
url: /it/net/aspose.tasks/yearlyrecurrencepattern/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern constructor

Inizializza una nuova istanza della classe [`YearlyRecurrencePattern`](../).

```csharp
public YearlyRecurrencePattern()
```

## Esempi

Mostra come lavorare con i modelli di ricorrenza annuale durante la creazione di attività ricorrenti.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "WorkWithYearlyRecurrencePattern_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


