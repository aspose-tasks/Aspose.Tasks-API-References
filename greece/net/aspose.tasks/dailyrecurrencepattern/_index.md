---
title: "Class DailyRecurrencePattern"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.DailyRecurrencePattern class. Αντιπροσωπεύει το σύνολο των παραμέτρων που χρησιμοποιούνται για τη δημιουργία μιας καθημερινής επαναλαμβανόμενης εργασίας σε ένα έργο"
type: docs
weight: 400
url: /el/net/aspose.tasks/dailyrecurrencepattern/
---
## DailyRecurrencePattern class

Αντιπροσωπεύει το σύνολο των παραμέτρων που χρησιμοποιούνται για τη δημιουργία μιας καθημερινής επαναλαμβανόμενης εργασίας σε ένα έργο.

```csharp
public class DailyRecurrencePattern : RecurrencePatternBase
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [DailyRecurrencePattern](dailyrecurrencepattern/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `DailyRecurrencePattern`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Λαμβάνει ή ορίζει το εύρος επανάληψης. |
| [Repetition](../../aspose.tasks/dailyrecurrencepattern/repetition/) { get; set; } | Λαμβάνει ή ορίζει το πρότυπο των επαναλήψεων στο καθημερινό πρότυπο επανάληψης. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


