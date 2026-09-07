---
title: "YearlyRecurrencePattern.YearlyRecurrencePattern"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής YearlyRecurrencePattern. Αρχικοποιεί μια νέα παρουσία της κλάσης YearlyRecurrencePattern"
type: docs
weight: 10
url: /el/net/aspose.tasks/yearlyrecurrencepattern/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`YearlyRecurrencePattern`](../).

```csharp
public YearlyRecurrencePattern()
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

* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


