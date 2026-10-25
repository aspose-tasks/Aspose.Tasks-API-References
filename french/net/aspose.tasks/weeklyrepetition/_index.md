---
title: "Classe WeeklyRepetition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.WeeklyRepetition. Représente un modèle basé sur les jours de la semaine"
type: docs
weight: 3590
url: /fr/net/aspose.tasks/weeklyrepetition/
---
## WeeklyRepetition class

Représente un modèle basé sur les jours de la semaine.

```csharp
public class WeeklyRepetition : WeeklyRepetitionBase
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WeeklyRepetition](weeklyrepetition/)() | Initialise une nouvelle instance de la classe `WeeklyRepetition`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | Obtient ou définit un nombre de semaines qui représente l'intervalle en semaines entre les occurrences. |
| [WeekDays](../../aspose.tasks/weeklyrepetition/weekdays/) { get; set; } | Obtient ou définit un type de jours de la semaine. |

## Exemples

Montre comment créer une tâche récurrente.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "Recurring task",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new WeeklyRecurrencePattern
                                                 {
                                                     Repetition = new WeeklyRepetition
                                                                      {
                                                                          RepetitionInterval = 2,
                                                                          WeekDays = WeekdayType.Sunday | WeekdayType.Monday | WeekdayType.Friday
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 7, 20, 17, 0, 0)
                                                                           }
                                                 },
                         IgnoreResourceCalendar = false
                     };

parameters.SetCalendar(project, "Standard");

project.RootTask.Children.Add(parameters);
```

### Voir aussi

* class [WeeklyRepetitionBase](../weeklyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


