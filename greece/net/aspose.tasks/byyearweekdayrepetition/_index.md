---
title: "Κλάση ByYearWeekDayRepetition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η κλάση Aspose.Tasks.ByYearWeekDayRepetition. Αντιπροσωπεύει ένα μοτίβο που βασίζεται στη θέση μιας ημέρας της εβδομάδας σε ένα μήνα"
type: docs
weight: 200
url: /el/net/aspose.tasks/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition class

Αντιπροσωπεύει ένα μοτίβο που βασίζεται στη θέση μιας ημέρας της εβδομάδας σε ένα μήνα.

```csharp
public class ByYearWeekDayRepetition : YearlyRepetitionBase
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ByYearWeekDayRepetition](byyearweekdayrepetition/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `ByYearWeekDayRepetition`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Month](../../aspose.tasks/byyearweekdayrepetition/month/) { get; set; } | Λαμβάνει ή ορίζει ένα μήνα στον οποίο η εργασία πρέπει να επαναλαμβάνεται. |
| [Position](../../aspose.tasks/byyearweekdayrepetition/position/) { get; set; } | Λαμβάνει ή ορίζει μια θέση της ημέρας σε μια εβδομάδα ενός μήνα στην οποία η εργασία πρέπει να επαναλαμβάνεται. |
| [WeekDay](../../aspose.tasks/byyearweekdayrepetition/weekday/) { get; set; } | Λαμβάνει ή ορίζει έναν τύπο ημέρας της εβδομάδας στην οποία η εργασία πρέπει να επαναλαμβάνεται. |

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

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


