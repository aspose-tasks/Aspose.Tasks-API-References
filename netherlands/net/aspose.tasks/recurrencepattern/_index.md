---
title: "Enum RecurrencePattern"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.RecurrencePattern enum. Vertegenwoordigt een type terugkeerpatroon van een terugkerende taak"
type: docs
weight: 1690
url: /nl/net/aspose.tasks/recurrencepattern/
---
## RecurrencePattern enumeration

Stelt een type herhalingspatroon van een terugkerende taak voor.

```csharp
[Flags]
public enum RecurrencePattern
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Daily | `1` | Dagelijks patroon. |
| Weekly | `4` | Wekelijks patroon. |
| Monthly | `8` | Maandelijks patroon. |
| Yearly | `10` | Jaarlijks patroon. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


