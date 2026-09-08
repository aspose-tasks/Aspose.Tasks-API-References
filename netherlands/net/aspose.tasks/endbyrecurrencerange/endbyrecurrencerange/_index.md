---
title: "EndByRecurrenceRange.EndByRecurrenceRange"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "EndByRecurrenceRange-constructor. Initialiseert een nieuwe instantie van de EndByRecurrenceRange-klasse."
type: docs
weight: 10
url: /nl/net/aspose.tasks/endbyrecurrencerange/endbyrecurrencerange/
---
## EndByRecurrenceRange constructor

Initialiseert een nieuwe instantie van de [`EndByRecurrenceRange`](../) klasse.

```csharp
public EndByRecurrenceRange()
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

* class [EndByRecurrenceRange](../)
* namespace [Aspose.Tasks](../../endbyrecurrencerange/)
* assembly [Aspose.Tasks](../../../)


