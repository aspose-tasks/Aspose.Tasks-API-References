---
title: "RecurringTaskParameters.RecurrencePattern"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα RecurringTaskParameters. Λαμβάνει ή ορίζει το πρότυπο επανάληψης της επαναλαμβανόμενης εργασίας. Μπορεί να είναι μία από τις τιμές της απαρίθμησης RecurrencePattern."
type: docs
weight: 40
url: /el/net/aspose.tasks/recurringtaskparameters/recurrencepattern/
---
## RecurringTaskParameters.RecurrencePattern property

Λαμβάνει ή ορίζει το πρότυπο επανάληψης της επαναλαμβανόμενης εργασίας. Μπορεί να είναι μία από τις τιμές της απαρίθμησης `RecurrencePattern`.

```csharp
public RecurrencePatternBase RecurrencePattern { get; set; }
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

* class [RecurrencePatternBase](../../recurrencepatternbase/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


