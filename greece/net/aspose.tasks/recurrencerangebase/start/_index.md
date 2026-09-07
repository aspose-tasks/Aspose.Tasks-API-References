---
title: "RecurrenceRangeBase.Start"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα RecurrenceRangeBase. Λαμβάνει ή ορίζει την ημερομηνία έναρξης του εύρους επανάληψης της επαναλαμβανόμενης εργασίας."
type: docs
weight: 10
url: /el/net/aspose.tasks/recurrencerangebase/start/
---
## RecurrenceRangeBase.Start property

Λαμβάνει ή ορίζει την ημερομηνία έναρξης του εύρους επανάληψης της επαναλαμβανόμενης εργασίας.

```csharp
public DateTime Start { get; set; }
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

* class [RecurrenceRangeBase](../)
* namespace [Aspose.Tasks](../../recurrencerangebase/)
* assembly [Aspose.Tasks](../../../)


