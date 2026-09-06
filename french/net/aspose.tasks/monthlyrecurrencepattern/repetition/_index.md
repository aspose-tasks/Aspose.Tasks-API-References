---
title: "MonthlyRecurrencePattern.Repetition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété MonthlyRecurrencePattern. Obtient ou définit le modèle de répétition récurrente"
type: docs
weight: 20
url: /fr/net/aspose.tasks/monthlyrecurrencepattern/repetition/
---
## MonthlyRecurrencePattern.Repetition property

Obtient ou définit le modèle de répétition récurrent.

```csharp
public MonthlyRepetitionBase Repetition { get; set; }
```

## Exemples

Montre comment travailler avec les répétitions de motif de récurrence mensuelle lors de la création de tâches récurrentes.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [MonthlyRepetitionBase](../../monthlyrepetitionbase/)
* class [MonthlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../monthlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


