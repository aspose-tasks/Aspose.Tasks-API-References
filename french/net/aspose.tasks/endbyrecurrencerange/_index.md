---
title: "Classe EndByRecurrenceRange"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.EndByRecurrenceRange. Représente la plage de récurrence d’une tâche récurrente qui est limitée par le jour de fin"
type: docs
weight: 510
url: /fr/net/aspose.tasks/endbyrecurrencerange/
---
## EndByRecurrenceRange class

Représente la plage de récurrence d'une tâche récurrente limitée par le jour de fin.

```csharp
public class EndByRecurrenceRange : RecurrenceRangeBase
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [EndByRecurrenceRange](endbyrecurrencerange/)() | Initialise une nouvelle instance de la classe `EndByRecurrenceRange`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Finish](../../aspose.tasks/endbyrecurrencerange/finish/) { get; set; } | Obtient ou définit la date qui limite la plage de récurrence de la tâche récurrente. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Obtient ou définit la date de début de la plage de récurrence de la tâche récurrente. |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


