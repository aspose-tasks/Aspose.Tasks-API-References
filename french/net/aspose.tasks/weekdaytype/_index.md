---
title: "Énum WeekdayType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Enum Aspose.Tasks.WeekdayType. Représente un jour de la semaine d’un projet dans l’instance de la classe RecurringTaskInfo."
type: docs
weight: 3570
url: /fr/net/aspose.tasks/weekdaytype/
---
## WeekdayType enumeration

Représente un jour de la semaine d’un projet dans l’instance de la classe [`RecurringTaskInfo`](../recurringtaskinfo/).

```csharp
[Flags]
public enum WeekdayType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Indique le type de jour de la semaine None. |
| Sunday | `1` | Indique le type de jour de la semaine Sunday. |
| Monday | `2` | Indique le type de jour de la semaine Monday. |
| Tuesday | `4` | Indique le type de jour de la semaine Tuesday. |
| Wednesday | `8` | Indique le type de jour de la semaine Wednesday. |
| Thursday | `10` | Indique le type de jour de la semaine Thursday. |
| Friday | `20` | Indique le type de jour de la semaine Friday. |
| Saturday | `40` | Indique le type de jour de la semaine Saturday. |

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


