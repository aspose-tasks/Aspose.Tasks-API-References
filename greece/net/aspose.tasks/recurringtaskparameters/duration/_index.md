---
title: "RecurringTaskParameters.Duration"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα RecurringTaskParameters. Λαμβάνει ή ορίζει τη διάρκεια για μία εμφάνιση της επαναλαμβανόμενης εργασίας. Το στιγμιότυπο της κλάσης Duration."
type: docs
weight: 20
url: /el/net/aspose.tasks/recurringtaskparameters/duration/
---
## RecurringTaskParameters.Duration property

Λαμβάνει ή ορίζει τη διάρκεια για μία εμφάνιση της επαναλαμβανόμενης εργασίας. Το στιγμιότυπο της κλάσης `Duration`.

```csharp
public Duration Duration { get; set; }
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

* struct [Duration](../../duration/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


