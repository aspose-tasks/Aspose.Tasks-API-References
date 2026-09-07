---
title: "Κλάση YearlyRecurrencePattern"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.YearlyRecurrencePattern κλάση. Αντιπροσωπεύει το σύνολο των παραμέτρων που χρησιμοποιούνται για τη δημιουργία ετήσιας επαναλαμβανόμενης εργασίας σε ένα έργο."
type: docs
weight: 3690
url: /el/net/aspose.tasks/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern class

Αντιπροσωπεύει το σύνολο των παραμέτρων που χρησιμοποιούνται για τη δημιουργία μιας ετήσιας επαναλαμβανόμενης εργασίας σε ένα έργο.

```csharp
public class YearlyRecurrencePattern : RecurrencePatternBase
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [YearlyRecurrencePattern](yearlyrecurrencepattern/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `YearlyRecurrencePattern`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Λαμβάνει ή ορίζει το εύρος επανάληψης. |
| [Repetition](../../aspose.tasks/yearlyrecurrencepattern/repetition/) { get; set; } | Λαμβάνει ή ορίζει το πρότυπο επαναλαμβανόμενης θέσης. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με πρότυπα επαναλαμβανόμενων ετών κατά τη δημιουργία επαναλαμβανόμενων εργασιών.

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

project.Save(OutDir + "WorkWithYearlyRecurrencePattern_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


