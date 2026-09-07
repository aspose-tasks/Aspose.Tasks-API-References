---
title: "DailyWorkRepetition.DailyWorkRepetition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής DailyWorkRepetition. Αρχικοποιεί μια νέα παρουσία της κλάσης DailyWorkRepetition"
type: docs
weight: 10
url: /el/net/aspose.tasks/dailyworkrepetition/dailyworkrepetition/
---
## DailyWorkRepetition constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`DailyWorkRepetition`](../).

```csharp
public DailyWorkRepetition()
```

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

* class [DailyWorkRepetition](../)
* namespace [Aspose.Tasks](../../dailyworkrepetition/)
* assembly [Aspose.Tasks](../../../)


