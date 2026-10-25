---
title: "Κλάση WeeklyRepetition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.WeeklyRepetition κλάση. Αντιπροσωπεύει ένα μοτίβο που βασίζεται σε ημέρες της εβδομάδας"
type: docs
weight: 3590
url: /el/net/aspose.tasks/weeklyrepetition/
---
## WeeklyRepetition class

Αντιπροσωπεύει ένα μοτίβο που βασίζεται σε ημέρες της εβδομάδας.

```csharp
public class WeeklyRepetition : WeeklyRepetitionBase
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [WeeklyRepetition](weeklyrepetition/)() | Αρχικοποιεί μια νέα παρουσία της `WeeklyRepetition` κλάσης. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | Λαμβάνει ή ορίζει έναν αριθμό εβδομάδων που αντιπροσωπεύει το διάστημα σε εβδομάδες μεταξύ των εμφανίσεων. |
| [WeekDays](../../aspose.tasks/weeklyrepetition/weekdays/) { get; set; } | Λαμβάνει ή ορίζει έναν τύπο ημερών της εβδομάδας. |

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

* class [WeeklyRepetitionBase](../weeklyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


