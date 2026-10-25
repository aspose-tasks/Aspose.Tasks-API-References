---
title: "DailyRecurrencePattern.DailyRecurrencePattern"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής DailyRecurrencePattern. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης DailyRecurrencePattern"
type: docs
weight: 10
url: /el/net/aspose.tasks/dailyrecurrencepattern/dailyrecurrencepattern/
---
## DailyRecurrencePattern constructor

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`DailyRecurrencePattern`](../).

```csharp
public DailyRecurrencePattern()
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

* class [DailyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../dailyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


