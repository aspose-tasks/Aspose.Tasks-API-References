---
title: "RecurringTaskParameters.SetCalendar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος RecurringTaskParameters. Ορίζει ένα ημερολόγιο για την επαναλαμβανόμενη εργασία. Το ημερολόγιο επιλέγεται από τη συλλογή ημερολογίων του έργου."
type: docs
weight: 60
url: /el/net/aspose.tasks/recurringtaskparameters/setcalendar/
---
## RecurringTaskParameters.SetCalendar method

Ορίστε ένα ημερολόγιο για την επαναλαμβανόμενη εργασία. Το ημερολόγιο επιλέγεται από τη συλλογή ημερολογίων του έργου.

```csharp
public void SetCalendar(Project project, string calendarName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| project | Project | Το έργο με τη συλλογή ημερολογίων. |
| calendarName | String | Το όνομα του ημερολογίου. |

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

* class [Project](../../project/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


