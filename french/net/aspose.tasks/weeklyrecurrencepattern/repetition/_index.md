---
title: "WeeklyRecurrencePattern.Repetition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété WeeklyRecurrencePattern. Obtient ou définit le modèle de répétition récurrente"
type: docs
weight: 20
url: /fr/net/aspose.tasks/weeklyrecurrencepattern/repetition/
---
## WeeklyRecurrencePattern.Repetition property

Obtient ou définit le modèle de répétition récurrent.

```csharp
public WeeklyRepetitionBase Repetition { get; set; }
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

* class [WeeklyRepetitionBase](../../weeklyrepetitionbase/)
* class [WeeklyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../weeklyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


