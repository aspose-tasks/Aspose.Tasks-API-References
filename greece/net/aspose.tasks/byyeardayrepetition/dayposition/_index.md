---
title: "ByYearDayRepetition.DayPosition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ByYearDayRepetition. Λαμβάνει ή ορίζει τη θέση της ημέρας σε ένα μήνα στον οποίο η εργασία πρέπει να επαναλαμβάνεται"
type: docs
weight: 20
url: /el/net/aspose.tasks/byyeardayrepetition/dayposition/
---
## ByYearDayRepetition.DayPosition property

Λαμβάνει ή ορίζει μια θέση ημέρας σε ένα μήνα στην οποία η εργασία πρέπει να επαναλαμβάνεται.

```csharp
public int DayPosition { get; set; }
```

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

* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


