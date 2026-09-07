---
title: "ByYearWeekDayRepetition.Position"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ByYearWeekDayRepetition. Λαμβάνει ή ορίζει τη θέση της ημέρας σε μια εβδομάδα ενός μήνα στην οποία η εργασία πρέπει να επαναλαμβάνεται"
type: docs
weight: 30
url: /el/net/aspose.tasks/byyearweekdayrepetition/position/
---
## ByYearWeekDayRepetition.Position property

Λαμβάνει ή ορίζει μια θέση της ημέρας σε μια εβδομάδα ενός μήνα στην οποία η εργασία πρέπει να επαναλαμβάνεται.

```csharp
public OrdinalNumber Position { get; set; }
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

* enum [OrdinalNumber](../../ordinalnumber/)
* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


