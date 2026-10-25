---
title: "Κλάση DailyWorkRepetition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.DailyWorkRepetition. Αντιπροσωπεύει μια κλάση για επαναλήψεις σε ημερήσιο πρότυπο επανάληψης βάσει εργάσιμων ημερών"
type: docs
weight: 420
url: /el/net/aspose.tasks/dailyworkrepetition/
---
## DailyWorkRepetition class

Αντιπροσωπεύει μια κλάση για επαναλήψεις σε καθημερινό μοτίβο επανάληψης βασισμένο σε εργάσιμες ημέρες.

```csharp
public class DailyWorkRepetition : DailyRepetitionBase
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [DailyWorkRepetition](dailyworkrepetition/)() | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `DailyWorkRepetition`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | Λαμβάνει ή ορίζει έναν αριθμό ημερών που αντιπροσωπεύει το διάστημα σε ημέρες μεταξύ των εμφανίσεων. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με επαναλήψεις προτύπου ημερήσιας εργασίας ενώ δημιουργείτε επαναλαμβανόμενες εργασίες.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "New recurrent task",
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     RecurrenceRange = new EndAfterRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 1, 1, 8, 0, 0), OccurrenceNumber = 9
                                                                           },
                                                     Repetition = new DailyWorkRepetition { RepetitionInterval = 1 }
                                                 },
                         Duration = project.GetDuration(1, TimeUnitType.Hour)
                     };
parameters.SetCalendar(project, "Standard");

var task = project.RootTask.Children.Add(parameters);
task.Set(Tsk.Start, new DateTime(2020, 4, 27, 8, 0, 0));

// συνεχίστε την εργασία με το έργο...
// ...
```

### Δείτε επίσης

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


