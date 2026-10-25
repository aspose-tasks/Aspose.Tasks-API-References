---
title: "Enum RecurringInterval.DayType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.RecurringIntervalDayType enum. Αντιπροσωπεύει έναν τύπο ημέρας που χρησιμοποιείται σε γραμμές προόδου"
type: docs
weight: 3320
url: /el/net/aspose.tasks.visualization/recurringinterval.daytype/
---
## RecurringInterval.DayType enumeration

Αντιπροσωπεύει έναν τύπο ημέρας που χρησιμοποιείται σε γραμμές προόδου.

```csharp
public enum DayType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Sunday | `1` | Δείχνει την Κυριακή. |
| Monday | `2` | Δείχνει τη Δευτέρα. |
| Tuesday | `3` | Δείχνει την Τρίτη. |
| Wednesday | `4` | Δείχνει την Τετάρτη. |
| Thursday | `5` | Δείχνει την Πέμπτη. |
| Friday | `6` | Δείχνει την Παρασκευή. |
| Saturday | `7` | Δείχνει το Σάββατο. |
| Day | `8` | Δείχνει Ημέρα. |
| Workday | `9` | Δείχνει Εργάσιμη ημέρα. |
| NonworkingDay | `10` | Δείχνει Μη εργάσιμη ημέρα. |

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

* class [RecurringInterval](../recurringinterval/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


