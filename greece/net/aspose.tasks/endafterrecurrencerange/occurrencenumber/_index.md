---
title: "EndAfterRecurrenceRange.OccurrenceNumber"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "EndAfterRecurrenceRange property. Λαμβάνει ή ορίζει τον αριθμό των εμφανίσεων που περιορίζει το εύρος επανάληψης της επαναλαμβανόμενης εργασίας"
type: docs
weight: 20
url: /el/net/aspose.tasks/endafterrecurrencerange/occurrencenumber/
---
## EndAfterRecurrenceRange.OccurrenceNumber property

Λαμβάνει ή ορίζει τον αριθμό εμφανίσεων που περιορίζει το εύρος επανάληψης της επαναλαμβανόμενης εργασίας.

```csharp
public int OccurrenceNumber { get; set; }
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

* class [EndAfterRecurrenceRange](../)
* namespace [Aspose.Tasks](../../endafterrecurrencerange/)
* assembly [Aspose.Tasks](../../../)


