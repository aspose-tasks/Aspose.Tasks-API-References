---
title: "Απαρίθμηση RecurrencePattern"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.RecurrencePattern enum. Αντιπροσωπεύει έναν τύπο προτύπου επανάληψης μιας επαναλαμβανόμενης εργασίας"
type: docs
weight: 1690
url: /el/net/aspose.tasks/recurrencepattern/
---
## RecurrencePattern enumeration

Αναπαριστά έναν τύπο προτύπου επανάληψης μιας επαναλαμβανόμενης εργασίας.

```csharp
[Flags]
public enum RecurrencePattern
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Daily | `1` | Καθημερινό πρότυπο. |
| Weekly | `4` | Εβδομαδιαίο πρότυπο. |
| Monthly | `8` | Μηνιαίο πρότυπο. |
| Yearly | `10` | Ετήσιο πρότυπο. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


