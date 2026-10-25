---
title: "ByYearDayRepetition.ByYearDayRepetition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής ByYearDayRepetition. Αρχικοποιεί μια νέα παρουσία της κλάσης ByYearDayRepetition"
type: docs
weight: 10
url: /el/net/aspose.tasks/byyeardayrepetition/byyeardayrepetition/
---
## ByYearDayRepetition constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`ByYearDayRepetition`](../).

```csharp
public ByYearDayRepetition()
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


