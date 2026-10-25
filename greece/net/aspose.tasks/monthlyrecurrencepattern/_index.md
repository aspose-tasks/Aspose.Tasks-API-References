---
title: "Κλάση MonthlyRecurrencePattern"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.MonthlyRecurrencePattern. Αντιπροσωπεύει το σύνολο των παραμέτρων που χρησιμοποιούνται για τη δημιουργία μιας μηνιαίας επαναλαμβανόμενης εργασίας σε ένα έργο."
type: docs
weight: 1080
url: /el/net/aspose.tasks/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern class

Αντιπροσωπεύει το σύνολο των παραμέτρων που χρησιμοποιούνται για τη δημιουργία μηνιαίας επαναλαμβανόμενης εργασίας σε ένα project.

```csharp
public class MonthlyRecurrencePattern : RecurrencePatternBase
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [MonthlyRecurrencePattern](monthlyrecurrencepattern/)() | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `MonthlyRecurrencePattern`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Λαμβάνει ή ορίζει το εύρος επανάληψης. |
| [Repetition](../../aspose.tasks/monthlyrecurrencepattern/repetition/) { get; set; } | Λαμβάνει ή ορίζει το επαναλαμβανόμενο μοτίβο επανάληψης. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με επαναλήψεις του μηνιαίου μοτίβου επανάληψης κατά τη δημιουργία επαναλαμβανόμενων εργασιών.

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


