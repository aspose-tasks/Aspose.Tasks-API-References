---
title: "YearlyRecurrencePattern.Repetition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα YearlyRecurrencePattern. Λαμβάνει ή ορίζει το μοτίβο επαναλαμβανόμενης θέσης"
type: docs
weight: 20
url: /el/net/aspose.tasks/yearlyrecurrencepattern/repetition/
---
## YearlyRecurrencePattern.Repetition property

Λαμβάνει ή ορίζει το πρότυπο επαναλαμβανόμενης θέσης.

```csharp
public YearlyRepetitionBase Repetition { get; set; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με πρότυπα επαναλαμβανόμενων ετών κατά τη δημιουργία επαναλαμβανόμενων εργασιών.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "WorkWithYearlyRecurrencePattern_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [YearlyRepetitionBase](../../yearlyrepetitionbase/)
* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


