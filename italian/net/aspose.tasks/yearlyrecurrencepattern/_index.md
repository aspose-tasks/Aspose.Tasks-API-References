---
title: "Classe YearlyRecurrencePattern"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.YearlyRecurrencePattern. Rappresenta l'insieme di parametri utilizzati per creare un'attività ricorrente annuale in un progetto"
type: docs
weight: 3690
url: /it/net/aspose.tasks/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern class

Rappresenta l'insieme dei parametri utilizzati per creare un'attività ricorrente annuale in un progetto.

```csharp
public class YearlyRecurrencePattern : RecurrencePatternBase
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [YearlyRecurrencePattern](yearlyrecurrencepattern/)() | Inizializza una nuova istanza della classe `YearlyRecurrencePattern`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Ottiene o imposta l'intervallo di ricorrenza. |
| [Repetition](../../aspose.tasks/yearlyrecurrencepattern/repetition/) { get; set; } | Ottiene o imposta il modello di posizione ricorrente. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


