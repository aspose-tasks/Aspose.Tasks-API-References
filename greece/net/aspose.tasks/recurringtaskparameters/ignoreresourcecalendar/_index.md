---
title: "RecurringTaskParameters.IgnoreResourceCalendar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα RecurringTaskParameters. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα προγραμματιστεί η επαναλαμβανόμενη εργασία ακόμη και όταν δεν υπάρχουν διαθέσιμοι πόροι για την εκτέλεσή της."
type: docs
weight: 30
url: /el/net/aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/
---
## RecurringTaskParameters.IgnoreResourceCalendar property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα προγραμματιστεί η επαναλαμβανόμενη εργασία ακόμη και αν δεν συμβαίνει όταν υπάρχουν διαθέσιμοι πόροι για να εργαστούν σε αυτήν.

```csharp
public bool IgnoreResourceCalendar { get; set; }
```

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

* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


