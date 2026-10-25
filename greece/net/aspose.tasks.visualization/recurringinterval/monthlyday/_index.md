---
title: "RecurringInterval.MonthlyDay"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα RecurringInterval. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται οι μηνιαίες γραμμές προόδου ανά ημέρα"
type: docs
weight: 50
url: /el/net/aspose.tasks.visualization/recurringinterval/monthlyday/
---
## RecurringInterval.MonthlyDay property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται οι μηνιαίες γραμμές προόδου ανά ημέρα.

```csharp
public bool MonthlyDay { get; set; }
```

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

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


