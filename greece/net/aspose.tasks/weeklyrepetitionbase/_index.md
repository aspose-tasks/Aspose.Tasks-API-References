---
title: "Κλάση WeeklyRepetitionBase"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η κλάση Aspose.Tasks.WeeklyRepetitionBase. Αντιπροσωπεύει μια βασική κλάση για επαναλήψεις σε εβδομαδιαίο πρότυπο επανάληψης"
type: docs
weight: 3600
url: /el/net/aspose.tasks/weeklyrepetitionbase/
---
## WeeklyRepetitionBase class

Αντιπροσωπεύει μια βασική κλάση για επαναλήψεις σε μοτίβο εβδομαδιαίας επανάληψης.

```csharp
public abstract class WeeklyRepetitionBase
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | Λαμβάνει ή ορίζει έναν αριθμό εβδομάδων που αντιπροσωπεύει το διάστημα σε εβδομάδες μεταξύ των εμφανίσεων. |

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


