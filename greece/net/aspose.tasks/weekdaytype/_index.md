---
title: "Απαρίθμηση WeekdayType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.WeekdayType enum. Αναπαριστά μια ημέρα της εβδομάδας ενός έργου στην περίπτωση της κλάσης RecurringTaskInfo."
type: docs
weight: 3570
url: /el/net/aspose.tasks/weekdaytype/
---
## WeekdayType enumeration

Αναπαριστά μια ημέρα της εβδομάδας ενός έργου στην περίπτωση της κλάσης [`RecurringTaskInfo`](../recurringtaskinfo/).

```csharp
[Flags]
public enum WeekdayType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| None | `0` | Δείχνει τύπο ημέρας None. |
| Sunday | `1` | Δείχνει τύπο ημέρας Κυριακή. |
| Monday | `2` | Δείχνει τύπο ημέρας Δευτέρα. |
| Tuesday | `4` | Δείχνει τύπο ημέρας Τρίτη. |
| Wednesday | `8` | Δείχνει τύπο ημέρας Τετάρτη. |
| Thursday | `10` | Δείχνει τύπο ημέρας Πέμπτη. |
| Friday | `20` | Δείχνει τύπο ημέρας Παρασκευή. |
| Saturday | `40` | Δείχνει τύπο ημέρας Σάββατο. |

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


