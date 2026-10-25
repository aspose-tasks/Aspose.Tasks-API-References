---
title: "Classe YearlyRepetitionBase"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.YearlyRepetitionBase. Rappresenta un modello di base per la posizione giornaliera annuale"
type: docs
weight: 3700
url: /it/net/aspose.tasks/yearlyrepetitionbase/
---
## YearlyRepetitionBase class

Rappresenta un modello base per la posizione giornaliera annuale.

```csharp
public abstract class YearlyRepetitionBase
```

## Esempi

Mostra come lavorare con le ripetizioni giornaliere annuali durante la creazione di nuove attività ricorrenti.

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

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


