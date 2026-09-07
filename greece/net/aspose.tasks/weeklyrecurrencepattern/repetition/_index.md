---
title: "WeeklyRecurrencePattern.Repetition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα WeeklyRecurrencePattern. Λαμβάνει ή ορίζει το επαναλαμβανόμενο μοτίβο επανάληψης"
type: docs
weight: 20
url: /el/net/aspose.tasks/weeklyrecurrencepattern/repetition/
---
## WeeklyRecurrencePattern.Repetition property

Λαμβάνει ή ορίζει το επαναλαμβανόμενο μοτίβο επανάληψης.

```csharp
public WeeklyRepetitionBase Repetition { get; set; }
```

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε μια επαναλαμβανόμενη εργασία.

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

### Δείτε επίσης

* class [WeeklyRepetitionBase](../../weeklyrepetitionbase/)
* class [WeeklyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../weeklyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


