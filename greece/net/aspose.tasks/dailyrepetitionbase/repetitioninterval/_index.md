---
title: "DailyRepetitionBase.RepetitionInterval"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα DailyRepetitionBase. Λαμβάνει ή ορίζει έναν αριθμό ημερών που αντιπροσωπεύει το διάστημα σε ημέρες μεταξύ των εμφανίσεων"
type: docs
weight: 10
url: /el/net/aspose.tasks/dailyrepetitionbase/repetitioninterval/
---
## DailyRepetitionBase.RepetitionInterval property

Λαμβάνει ή ορίζει έναν αριθμό ημερών που αντιπροσωπεύει το διάστημα σε ημέρες μεταξύ των εμφανίσεων.

```csharp
public int RepetitionInterval { get; set; }
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

* class [DailyRepetitionBase](../)
* namespace [Aspose.Tasks](../../dailyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


