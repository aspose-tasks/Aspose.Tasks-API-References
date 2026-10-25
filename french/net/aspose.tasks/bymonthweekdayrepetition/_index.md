---
title: "Classe ByMonthWeekDayRepetition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ByMonthWeekDayRepetition. Représente un modèle basé sur la position du jour de la semaine dans un mois"
type: docs
weight: 180
url: /fr/net/aspose.tasks/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition class

Représente un modèle basé sur la position du jour de la semaine dans un mois.

```csharp
public class ByMonthWeekDayRepetition : MonthlyRepetitionBase
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ByMonthWeekDayRepetition](bymonthweekdayrepetition/)() | Initialise une nouvelle instance de la classe `ByMonthWeekDayRepetition`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Position](../../aspose.tasks/bymonthweekdayrepetition/position/) { get; set; } | Obtient ou définit une position du jour de la semaine dans un mois où la tâche doit se répéter. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Obtient ou définit le nombre de mois qui représente l'intervalle en mois entre les occurrences. |
| [WeekDay](../../aspose.tasks/bymonthweekdayrepetition/weekday/) { get; set; } | Obtient ou définit un type de jour de la semaine sur lequel la tâche doit se répéter. |

## Exemples

Montre comment travailler avec les répétitions de jours de semaine mensuels lors de la création de nouvelles tâches récurrentes.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthWeekDayRepetition
                                                                      {
                                                                          Position = OrdinalNumber.First,
                                                                          WeekDay = DayOfWeek.Sunday,
                                                                          RepetitionInterval = 2
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 2, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);
project.Save(OutDir + "CanAddRecurringTask_Months_WeekDay_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


