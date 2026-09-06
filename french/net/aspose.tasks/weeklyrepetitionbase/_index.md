---
title: "Classe WeeklyRepetitionBase"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.WeeklyRepetitionBase. Représente une classe de base pour les répétitions dans un modèle de récurrence hebdomadaire"
type: docs
weight: 3600
url: /fr/net/aspose.tasks/weeklyrepetitionbase/
---
## WeeklyRepetitionBase class

Représente une classe de base pour les répétitions dans le modèle de récurrence hebdomadaire.

```csharp
public abstract class WeeklyRepetitionBase
```

## Propriétés

| Nom | Description |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | Obtient ou définit un nombre de semaines qui représente l'intervalle en semaines entre les occurrences. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


