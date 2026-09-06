---
title: "Classe ByYearWeekDayRepetition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ByYearWeekDayRepetition. Représente un modèle basé sur la position d'un jour de la semaine dans un mois"
type: docs
weight: 200
url: /fr/net/aspose.tasks/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition class

Représente un modèle basé sur la position d'un jour de la semaine dans un mois.

```csharp
public class ByYearWeekDayRepetition : YearlyRepetitionBase
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ByYearWeekDayRepetition](byyearweekdayrepetition/)() | Initialise une nouvelle instance de la classe `ByYearWeekDayRepetition`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Month](../../aspose.tasks/byyearweekdayrepetition/month/) { get; set; } | Obtient ou définit le mois pendant lequel la tâche doit être récurrente. |
| [Position](../../aspose.tasks/byyearweekdayrepetition/position/) { get; set; } | Obtient ou définit la position du jour dans une semaine d'un mois pendant lequel la tâche doit être récurrente. |
| [WeekDay](../../aspose.tasks/byyearweekdayrepetition/weekday/) { get; set; } | Obtient ou définit le type de jour de la semaine auquel la tâche doit être récurrente. |

## Exemples

Montre comment travailler avec les répétitions de jours de la semaine sur une année lors de la création de nouvelles tâches récurrentes.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearWeekDayRepetition
                                                                      {
                                                                          Month = Month.July, WeekDay = DayOfWeek.Sunday, Position = OrdinalNumber.First
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 31, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearWeekDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


