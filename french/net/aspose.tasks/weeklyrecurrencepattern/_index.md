---
title: "Classe WeeklyRecurrencePattern"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.WeeklyRecurrencePattern. Représente l'ensemble des paramètres utilisés pour créer une tâche récurrente hebdomadaire dans un projet"
type: docs
weight: 3580
url: /fr/net/aspose.tasks/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern class

Représente l'ensemble des paramètres utilisés pour créer une tâche récurrente hebdomadaire dans un projet.

```csharp
public class WeeklyRecurrencePattern : RecurrencePatternBase
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WeeklyRecurrencePattern](weeklyrecurrencepattern/)() | Initialise une nouvelle instance de la classe `WeeklyRecurrencePattern`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Obtient ou définit la plage de récurrence. |
| [Repetition](../../aspose.tasks/weeklyrecurrencepattern/repetition/) { get; set; } | Obtient ou définit le modèle de répétition récurrent. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


