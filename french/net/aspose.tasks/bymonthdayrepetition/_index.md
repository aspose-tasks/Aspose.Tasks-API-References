---
title: "Class ByMonthDayRepetition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ByMonthDayRepetition. Représente un modèle basé sur la position absolue d'un jour dans un mois"
type: docs
weight: 170
url: /fr/net/aspose.tasks/bymonthdayrepetition/
---
## ByMonthDayRepetition class

Représente un modèle basé sur la position absolue d'un jour dans un mois.

```csharp
public class ByMonthDayRepetition : MonthlyRepetitionBase
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ByMonthDayRepetition](bymonthdayrepetition/)() | Initialise une nouvelle instance de la classe `ByMonthDayRepetition`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [DayPosition](../../aspose.tasks/bymonthdayrepetition/dayposition/) { get; set; } | Obtient ou définit la position d'un jour dans un mois où la tâche doit être récurrente. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Obtient ou définit le nombre de mois qui représente l'intervalle en mois entre les occurrences. |

## Exemples

Montre comment travailler avec les répétitions de jour du mois lors de la création de nouvelles tâches récurrentes.

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


