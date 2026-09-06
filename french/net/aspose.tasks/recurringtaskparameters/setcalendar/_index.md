---
title: "RecurringTaskParameters.SetCalendar"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode RecurringTaskParameters. Définit un calendrier pour la tâche récurrente. Le calendrier est sélectionné dans la collection de calendriers du projet"
type: docs
weight: 60
url: /fr/net/aspose.tasks/recurringtaskparameters/setcalendar/
---
## RecurringTaskParameters.SetCalendar method

Définissez un calendrier pour la tâche récurrente. Le calendrier est sélectionné dans la collection de calendriers du projet.

```csharp
public void SetCalendar(Project project, string calendarName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| project | Project | Le projet avec la collection de calendriers. |
| calendarName | Chaîne | Le nom du calendrier. |

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

* class [Project](../../project/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


