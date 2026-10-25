---
title: "ByMonthWeekDayRepetition.WeekDay"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ByMonthWeekDayRepetition. Λαμβάνει ή ορίζει έναν τύπο ημέρας της εβδομάδας που η εργασία πρέπει να επαναλαμβάνεται"
type: docs
weight: 30
url: /el/net/aspose.tasks/bymonthweekdayrepetition/weekday/
---
## ByMonthWeekDayRepetition.WeekDay property

Λαμβάνει ή ορίζει έναν τύπο ημέρας της εβδομάδας στην οποία η εργασία πρέπει να επαναλαμβάνεται.

```csharp
public DayOfWeek WeekDay { get; set; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με επαναλήψεις ημέρας της εβδομάδας του μήνα ενώ δημιουργείτε νέες επαναλαμβανόμενες εργασίες.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthWeekDayRepetition
                                                                      {
                                                                          Position = OrdinalNumber.First,
                                                                          WeekDay = DayOfWeek.Sunday,
                                                                          RepetitionInterval = 2
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 2, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);
project.Save(OutDir + "CanAddRecurringTask_Months_WeekDay_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [ByMonthWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


