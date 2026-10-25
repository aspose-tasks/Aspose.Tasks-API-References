---
title: "Κλάση ByMonthWeekDayRepetition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η κλάση Aspose.Tasks.ByMonthWeekDayRepetition. Αντιπροσωπεύει ένα μοτίβο που βασίζεται στη θέση της ημέρας της εβδομάδας σε ένα μήνα"
type: docs
weight: 180
url: /el/net/aspose.tasks/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition class

Αντιπροσωπεύει ένα μοτίβο που βασίζεται στη θέση της ημέρας της εβδομάδας σε ένα μήνα.

```csharp
public class ByMonthWeekDayRepetition : MonthlyRepetitionBase
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ByMonthWeekDayRepetition](bymonthweekdayrepetition/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `ByMonthWeekDayRepetition`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Position](../../aspose.tasks/bymonthweekdayrepetition/position/) { get; set; } | Λαμβάνει ή ορίζει μια θέση της ημέρας της εβδομάδας σε ένα μήνα στην οποία η εργασία πρέπει να επαναλαμβάνεται. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό των μηνών που αντιπροσωπεύει το διάστημα σε μήνες μεταξύ των εμφανίσεων. |
| [WeekDay](../../aspose.tasks/bymonthweekdayrepetition/weekday/) { get; set; } | Λαμβάνει ή ορίζει έναν τύπο ημέρας της εβδομάδας στην οποία η εργασία πρέπει να επαναλαμβάνεται. |

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


