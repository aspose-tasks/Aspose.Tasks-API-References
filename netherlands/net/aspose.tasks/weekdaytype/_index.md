---
title: "Enum WeekdayType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.WeekdayType enum. Stelt een weekdag van een project voor in de instantie van de RecurringTaskInfo-klasse."
type: docs
weight: 3570
url: /nl/net/aspose.tasks/weekdaytype/
---
## WeekdayType enumeration

Stelt een weekdag van een project voor in de instantie van de [`RecurringTaskInfo`](../recurringtaskinfo/) klasse.

```csharp
[Flags]
public enum WeekdayType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| None | `0` | Geeft het type None-weekdag aan. |
| Sunday | `1` | Geeft het type zondag-weekdag aan. |
| Monday | `2` | Geeft het type maandag-weekdag aan. |
| Tuesday | `4` | Geeft het type dinsdag-weekdag aan. |
| Wednesday | `8` | Geeft het type woensdag-weekdag aan. |
| Thursday | `10` | Geeft het type donderdag-weekdag aan. |
| Friday | `20` | Geeft het type vrijdag-weekdag aan. |
| Saturday | `40` | Geeft het type zaterdag-weekdag aan. |

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


