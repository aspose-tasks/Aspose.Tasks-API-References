---
title: "RecurringTaskParameters.IgnoreResourceCalendar"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété RecurringTaskParameters. Obtient ou définit une valeur indiquant s'il faut planifier la tâche récurrente même si aucune ressource n'est disponible pour y travailler"
type: docs
weight: 30
url: /fr/net/aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/
---
## RecurringTaskParameters.IgnoreResourceCalendar property

Obtient ou définit une valeur indiquant s'il faut planifier la tâche récurrente même si aucune ressource n'est disponible pour travailler dessus.

```csharp
public bool IgnoreResourceCalendar { get; set; }
```

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

* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


