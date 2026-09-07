---
title: "Κλάση EndByRecurrenceRange"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.EndByRecurrenceRange κλάση. Αντιπροσωπεύει το εύρος επανάληψης μιας επαναλαμβανόμενης εργασίας που περιορίζεται από την ημέρα λήξης."
type: docs
weight: 510
url: /el/net/aspose.tasks/endbyrecurrencerange/
---
## EndByRecurrenceRange class

Αντιπροσωπεύει το εύρος επανάληψης μιας επαναλαμβανόμενης εργασίας που περιορίζεται από την ημέρα λήξης.

```csharp
public class EndByRecurrenceRange : RecurrenceRangeBase
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [EndByRecurrenceRange](endbyrecurrencerange/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `EndByRecurrenceRange`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Finish](../../aspose.tasks/endbyrecurrencerange/finish/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία που περιορίζει το εύρος επανάληψης της επαναλαμβανόμενης εργασίας. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία έναρξης του εύρους επανάληψης της επαναλαμβανόμενης εργασίας. |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


