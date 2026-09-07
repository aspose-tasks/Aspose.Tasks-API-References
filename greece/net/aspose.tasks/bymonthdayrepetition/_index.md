---
title: "Κλάση ByMonthDayRepetition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.ByMonthDayRepetition. Αντιπροσωπεύει ένα μοτίβο που βασίζεται στην απόλυτη θέση μιας ημέρας σε ένα μήνα"
type: docs
weight: 170
url: /el/net/aspose.tasks/bymonthdayrepetition/
---
## ByMonthDayRepetition class

Αντιπροσωπεύει ένα μοτίβο που βασίζεται στην απόλυτη θέση μιας ημέρας σε ένα μήνα.

```csharp
public class ByMonthDayRepetition : MonthlyRepetitionBase
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ByMonthDayRepetition](bymonthdayrepetition/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `ByMonthDayRepetition`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [DayPosition](../../aspose.tasks/bymonthdayrepetition/dayposition/) { get; set; } | Λαμβάνει ή ορίζει τη θέση μιας ημέρας σε ένα μήνα στην οποία η εργασία πρέπει να επαναλαμβάνεται. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό των μηνών που αντιπροσωπεύει το διάστημα σε μήνες μεταξύ των εμφανίσεων. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με επαναλήψεις ημέρας μήνα κατά τη δημιουργία νέων επαναλαμβανόμενων εργασιών.

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


