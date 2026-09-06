---
title: "Classe RecurringTaskParameters"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.RecurringTaskParameters. Représente l'ensemble des paramètres utilisés pour créer une tâche récurrente dans un projet"
type: docs
weight: 1730
url: /fr/net/aspose.tasks/recurringtaskparameters/
---
## RecurringTaskParameters class

Représente l'ensemble des paramètres utilisés pour créer une tâche récurrente dans un projet.

```csharp
public class RecurringTaskParameters
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [RecurringTaskParameters](recurringtaskparameters/)() | Initialise une nouvelle instance de la classe `RecurringTaskParameters`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Duration](../../aspose.tasks/recurringtaskparameters/duration/) { get; set; } | Obtient ou définit la durée d'une occurrence de la tâche récurrente. L'instance de la classe [`Duration`](./duration/). |
| [IgnoreResourceCalendar](../../aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut planifier la tâche récurrente même si aucune ressource n'est disponible pour travailler dessus. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskparameters/recurrencepattern/) { get; set; } | Obtient ou définit le modèle de récurrence de la tâche récurrente. Peut être l'une des valeurs de l'énumération [`RecurrencePattern`](./recurrencepattern/). |
| [TaskName](../../aspose.tasks/recurringtaskparameters/taskname/) { get; set; } | Obtient ou définit le nom de la tâche récurrente. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetCalendar](../../aspose.tasks/recurringtaskparameters/setcalendar/)(Project, string) | Définissez un calendrier pour la tâche récurrente. Le calendrier est sélectionné dans la collection de calendriers du projet. |

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


