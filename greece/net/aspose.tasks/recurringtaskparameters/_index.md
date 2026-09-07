---
title: "Κλάση RecurringTaskParameters"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.RecurringTaskParameters κλάση. Αντιπροσωπεύει το σύνολο των παραμέτρων που χρησιμοποιούνται για τη δημιουργία επαναλαμβανόμενης εργασίας σε ένα έργο"
type: docs
weight: 1730
url: /el/net/aspose.tasks/recurringtaskparameters/
---
## RecurringTaskParameters class

Αντιπροσωπεύει το σύνολο των παραμέτρων που χρησιμοποιούνται για τη δημιουργία μιας επαναλαμβανόμενης εργασίας σε ένα έργο.

```csharp
public class RecurringTaskParameters
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [RecurringTaskParameters](recurringtaskparameters/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `RecurringTaskParameters`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Duration](../../aspose.tasks/recurringtaskparameters/duration/) { get; set; } | Λαμβάνει ή ορίζει τη διάρκεια για μία εμφάνιση της επαναλαμβανόμενης εργασίας. Η παρουσία της κλάσης [`Duration`](./duration/). |
| [IgnoreResourceCalendar](../../aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα προγραμματιστεί η επαναλαμβανόμενη εργασία ακόμη και αν δεν συμβαίνει όταν υπάρχουν διαθέσιμοι πόροι για να εργαστούν σε αυτήν. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskparameters/recurrencepattern/) { get; set; } | Λαμβάνει ή ορίζει το πρότυπο επανάληψης της επαναλαμβανόμενης εργασίας. Μπορεί να είναι μία από τις τιμές της απαρίθμησης [`RecurrencePattern`](./recurrencepattern/). |
| [TaskName](../../aspose.tasks/recurringtaskparameters/taskname/) { get; set; } | Λαμβάνει ή ορίζει το όνομα της επαναλαμβανόμενης εργασίας. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [SetCalendar](../../aspose.tasks/recurringtaskparameters/setcalendar/)(Project, string) | Ορίστε ένα ημερολόγιο για την επαναλαμβανόμενη εργασία. Το ημερολόγιο επιλέγεται από τη συλλογή ημερολογίων του έργου. |

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


