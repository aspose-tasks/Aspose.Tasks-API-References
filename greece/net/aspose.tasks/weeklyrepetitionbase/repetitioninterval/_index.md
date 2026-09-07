---
title: "WeeklyRepetitionBase.RepetitionInterval"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα WeeklyRepetitionBase. Λαμβάνει ή ορίζει έναν αριθμό εβδομάδων που αντιπροσωπεύει το διάστημα σε εβδομάδες μεταξύ των εμφανίσεων"
type: docs
weight: 10
url: /el/net/aspose.tasks/weeklyrepetitionbase/repetitioninterval/
---
## WeeklyRepetitionBase.RepetitionInterval property

Λαμβάνει ή ορίζει έναν αριθμό εβδομάδων που αντιπροσωπεύει το διάστημα σε εβδομάδες μεταξύ των εμφανίσεων.

```csharp
public int RepetitionInterval { get; set; }
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

* class [WeeklyRepetitionBase](../)
* namespace [Aspose.Tasks](../../weeklyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


