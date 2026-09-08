---
title: "RecurringTaskParameters.Duration"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "RecurringTaskParameters eigenschap. Haalt de duur voor één uitvoering van de terugkerende taak op of stelt deze in. Het exemplaar van de Duration-klasse."
type: docs
weight: 20
url: /nl/net/aspose.tasks/recurringtaskparameters/duration/
---
## RecurringTaskParameters.Duration property

Haalt de duur voor één uitvoering van de terugkerende taak op of stelt deze in. Het exemplaar van de `Duration` klasse.

```csharp
public Duration Duration { get; set; }
```

## Voorbeelden

Toont hoe een terugkerende taak te maken.

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

### Zie ook

* struct [Duration](../../duration/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


