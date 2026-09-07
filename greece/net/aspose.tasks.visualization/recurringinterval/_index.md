---
title: "Κλάση RecurringInterval"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.RecurringInterval κλάση. Αντιπροσωπεύει επαναλαμβανόμενα διαστήματα που χρησιμοποιούνται σε γραμμές προόδου μιας προβολής Gantt Chart."
type: docs
weight: 3310
url: /el/net/aspose.tasks.visualization/recurringinterval/
---
## RecurringInterval class

Αναπαριστά επαναλαμβανόμενα διαστήματα που χρησιμοποιούνται στις γραμμές προόδου μιας προβολής Gantt Chart.

```csharp
public class RecurringInterval
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [RecurringInterval](recurringinterval/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [DailyDayNumber](../../aspose.tasks.visualization/recurringinterval/dailydaynumber/) { get; set; } | Λαμβάνει ή ορίζει τον ημερήσιο αριθμό ημέρας. |
| [DailyWorkday](../../aspose.tasks.visualization/recurringinterval/dailyworkday/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν μια ημέρα είναι εργάσιμη για τις ημερήσιες γραμμές προόδου. |
| [Interval](../../aspose.tasks.visualization/recurringinterval/interval/) { get; set; } | Λαμβάνει ή ορίζει το επαναλαμβανόμενο διάστημα. Μπορεί να είναι οποιαδήποτε τιμή του τύπου [`Interval`](./interval/). |
| [MonthlyDay](../../aspose.tasks.visualization/recurringinterval/monthlyday/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται οι μηνιαίες γραμμές προόδου ανά ημέρα. |
| [MonthlyDayDayNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaydaynumber/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό ημέρας των μηνιαίων γραμμών προόδου. |
| [MonthlyDayMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό μήνα των μηνιαίων γραμμών προόδου. |
| [MonthlyFirstLast](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlast/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται οι γραμμές προόδου με την πρώτη ή την τελευταία προκαθορισμένη ημέρα. |
| [MonthlyFirstLastDay](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastday/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο της πρώτης ή της τελευταίας ημέρας των μηνιαίων γραμμών προόδου. |
| [MonthlyFirstLastMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastmonthnumber/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό μήνα των γραμμών προόδου, που εμφανίζονται με την πρώτη ή την τελευταία προκαθορισμένη ημέρα. |
| [WeeklyDays](../../aspose.tasks.visualization/recurringinterval/weeklydays/) { get; } | Λαμβάνει μια λίστα ημερών για τις εβδομαδιαίες γραμμές προόδου. |
| [WeeklyWeekNumber](../../aspose.tasks.visualization/recurringinterval/weeklyweeknumber/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό εβδομάδας για τις εβδομαδιαίες γραμμές προόδου. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με επαναλαμβανόμενο διάστημα γραμμών προόδου.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

// επιτρέπει την ανάγνωση της γραμμής προόδου
var interval = view.ProgressLines.RecurringInterval;

Console.WriteLine("Interval: " + interval.Interval);
Console.WriteLine("Weekly Week Number: " + interval.WeeklyWeekNumber);
foreach (var day in interval.WeeklyDays)
{
    Console.WriteLine("Week day: " + day);
}

// επιτρέπει τον επαναπροσδιορισμό του επαναλαμβανόμενου διαστήματος
var newInterval = new RecurringInterval();

// ορίστε μια τιμή που υποδεικνύει αν θα εμφανίζονται μηνιαίες γραμμές προόδου ανά ημέρα.
interval.MonthlyDay = true;
// ορίστε τον αριθμό ημέρας των μηνιαίων γραμμών προόδου.
interval.MonthlyDayDayNumber = 1;
// ορίστε τον αριθμό μήνα των μηνιαίων γραμμών προόδου.
interval.MonthlyDayMonthNumber = 1;
// ορίστε μια τιμή που υποδεικνύει αν θα εμφανίζονται γραμμές προόδου με την πρώτη ή την τελευταία προκαθορισμένη ημέρα.
interval.MonthlyFirstLast = true;
// ορίστε τον τύπο της πρώτης ή της τελευταίας ημέρας των μηνιαίων γραμμών προόδου.
interval.MonthlyFirstLastDay = RecurringInterval.DayType.Day;
// ορίστε τον αριθμό μήνα των γραμμών προόδου, που εμφανίζονται με την πρώτη ή την τελευταία προκαθορισμένη ημέρα.
interval.MonthlyFirstLastMonthNumber = 1;

view.ProgressLines.RecurringInterval = newInterval;

project.Save(OutDir + "WorkWithRecurringInterval_out.pdf", SaveFileFormat.Pdf);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


