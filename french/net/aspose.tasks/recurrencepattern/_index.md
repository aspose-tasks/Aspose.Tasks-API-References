---
title: "Énumération RecurrencePattern"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.RecurrencePattern. Représente un type de modèle de récurrence d'une tâche récurrente."
type: docs
weight: 1690
url: /fr/net/aspose.tasks/recurrencepattern/
---
## RecurrencePattern enumeration

Représente un type de modèle de récurrence d'une tâche récurrente.

```csharp
[Flags]
public enum RecurrencePattern
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Daily | `1` | Modèle quotidien. |
| Weekly | `4` | Modèle hebdomadaire. |
| Monthly | `8` | Modèle mensuel. |
| Yearly | `10` | Modèle annuel. |

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


