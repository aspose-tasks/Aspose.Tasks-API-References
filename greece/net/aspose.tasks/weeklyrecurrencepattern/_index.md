---
title: "Κλάση WeeklyRecurrencePattern"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.WeeklyRecurrencePattern κλάση. Αναπαριστά το σύνολο των παραμέτρων που χρησιμοποιούνται για τη δημιουργία μιας εβδομαδιαίας επαναλαμβανόμενης εργασίας σε ένα έργο"
type: docs
weight: 3580
url: /el/net/aspose.tasks/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern class

Αντιπροσωπεύει το σύνολο των παραμέτρων που χρησιμοποιούνται για τη δημιουργία μιας εβδομαδιαίας επαναλαμβανόμενης εργασίας σε ένα έργο.

```csharp
public class WeeklyRecurrencePattern : RecurrencePatternBase
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [WeeklyRecurrencePattern](weeklyrecurrencepattern/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `WeeklyRecurrencePattern`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Λαμβάνει ή ορίζει το εύρος επανάληψης. |
| [Repetition](../../aspose.tasks/weeklyrecurrencepattern/repetition/) { get; set; } | Λαμβάνει ή ορίζει το επαναλαμβανόμενο μοτίβο επανάληψης. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


