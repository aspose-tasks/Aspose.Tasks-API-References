---
title: "Classe MonthlyRepetitionBase"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.MonthlyRepetitionBase. Représente un motif de base pour la position du jour mensuel"
type: docs
weight: 1090
url: /fr/net/aspose.tasks/monthlyrepetitionbase/
---
## MonthlyRepetitionBase class

Représente un modèle de base pour la position du jour mensuel.

```csharp
public abstract class MonthlyRepetitionBase
```

## Propriétés

| Nom | Description |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Obtient ou définit le nombre de mois qui représente l'intervalle en mois entre les occurrences. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


