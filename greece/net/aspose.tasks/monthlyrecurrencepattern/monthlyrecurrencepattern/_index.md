---
title: "MonthlyRecurrencePattern.MonthlyRecurrencePattern"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής MonthlyRecurrencePattern. Αρχικοποιεί μια νέα παρουσία της κλάσης MonthlyRecurrencePattern"
type: docs
weight: 10
url: /el/net/aspose.tasks/monthlyrecurrencepattern/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`MonthlyRecurrencePattern`](../).

```csharp
public MonthlyRecurrencePattern()
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με επαναλήψεις του μηνιαίου μοτίβου επανάληψης κατά τη δημιουργία επαναλαμβανόμενων εργασιών.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [MonthlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../monthlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


