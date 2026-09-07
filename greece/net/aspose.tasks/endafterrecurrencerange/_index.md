---
title: "Κλάση EndAfterRecurrenceRange"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.EndAfterRecurrenceRange class. Αναπαριστά το εύρος επανάληψης μιας επαναλαμβανόμενης εργασίας που περιορίζεται από τον αριθμό εμφανίσεων"
type: docs
weight: 500
url: /el/net/aspose.tasks/endafterrecurrencerange/
---
## EndAfterRecurrenceRange class

Αντιπροσωπεύει το εύρος επανάληψης μιας επαναλαμβανόμενης εργασίας που περιορίζεται από τον αριθμό των εμφανίσεων.

```csharp
public class EndAfterRecurrenceRange : RecurrenceRangeBase
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [EndAfterRecurrenceRange](endafterrecurrencerange/)() | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `EndAfterRecurrenceRange`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [OccurrenceNumber](../../aspose.tasks/endafterrecurrencerange/occurrencenumber/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό εμφανίσεων που περιορίζει το εύρος επανάληψης της επαναλαμβανόμενης εργασίας. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία έναρξης του εύρους επανάληψης της επαναλαμβανόμενης εργασίας. |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


