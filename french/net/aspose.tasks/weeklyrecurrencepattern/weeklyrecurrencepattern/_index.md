---
title: "WeeklyRecurrencePattern.WeeklyRecurrencePattern"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur WeeklyRecurrencePattern. Initialise une nouvelle instance de la classe WeeklyRecurrencePattern"
type: docs
weight: 10
url: /fr/net/aspose.tasks/weeklyrecurrencepattern/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern constructor

Initialise une nouvelle instance de la classe [`WeeklyRecurrencePattern`](../).

```csharp
public WeeklyRecurrencePattern()
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

* class [WeeklyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../weeklyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


