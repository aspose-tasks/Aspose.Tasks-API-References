---
title: "Κλάση ByYearDayRepetition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.ByYearDayRepetition. Αντιπροσωπεύει ένα πρότυπο που βασίζεται στην απόλυτη θέση μιας ημέρας σε ένα μήνα"
type: docs
weight: 190
url: /el/net/aspose.tasks/byyeardayrepetition/
---
## ByYearDayRepetition class

Αντιπροσωπεύει ένα μοτίβο που βασίζεται στην απόλυτη θέση μιας ημέρας σε ένα μήνα.

```csharp
public class ByYearDayRepetition : YearlyRepetitionBase
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ByYearDayRepetition](byyeardayrepetition/)() | Αρχικοποιεί ένα νέο παράδειγμα της κλάσης `ByYearDayRepetition`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [DayPosition](../../aspose.tasks/byyeardayrepetition/dayposition/) { get; set; } | Λαμβάνει ή ορίζει μια θέση ημέρας σε ένα μήνα στην οποία η εργασία πρέπει να επαναλαμβάνεται. |
| [Month](../../aspose.tasks/byyeardayrepetition/month/) { get; set; } | Λαμβάνει ή ορίζει ένα μήνα στον οποίο η εργασία πρέπει να επαναλαμβάνεται. |

## Παραδείγματα

Εμφανίζει πώς να εργαστείτε με επαναλήψεις ημερών του έτους ενώ δημιουργείτε νέες επαναλαμβανόμενες εργασίες.

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

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


