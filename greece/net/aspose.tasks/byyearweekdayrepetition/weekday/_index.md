---
title: "ByYearWeekDayRepetition.WeekDay"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ByYearWeekDayRepetition. Λαμβάνει ή ορίζει έναν τύπο ημέρας της εβδομάδας στην οποία η εργασία πρέπει να επαναλαμβάνεται"
type: docs
weight: 40
url: /el/net/aspose.tasks/byyearweekdayrepetition/weekday/
---
## ByYearWeekDayRepetition.WeekDay property

Λαμβάνει ή ορίζει έναν τύπο ημέρας της εβδομάδας στην οποία η εργασία πρέπει να επαναλαμβάνεται.

```csharp
public DayOfWeek WeekDay { get; set; }
```

## Παραδείγματα

Δείχνει πώς να εργάζεστε με επαναλήψεις ημέρας της εβδομάδας κατά το έτος κατά τη δημιουργία νέων επαναλαμβανόμενων εργασιών.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearWeekDayRepetition
                                                                      {
                                                                          Month = Month.July, WeekDay = DayOfWeek.Sunday, Position = OrdinalNumber.First
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 31, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearWeekDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


