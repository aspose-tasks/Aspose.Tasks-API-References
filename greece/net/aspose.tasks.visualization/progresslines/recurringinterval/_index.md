---
title: "ProgressLines.RecurringInterval"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ProgressLines. Αποκτά ή ορίζει το επαναλαμβανόμενο διάστημα. RecurringInterval"
type: docs
weight: 180
url: /el/net/aspose.tasks.visualization/progresslines/recurringinterval/
---
## ProgressLines.RecurringInterval property

Αποκτά ή ορίζει το επαναλαμβανόμενο διάστημα. `RecurringInterval`.

```csharp
public RecurringInterval RecurringInterval { get; set; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με γραμμές προόδου.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// ορίζουμε τη γραμμή προόδου
view.ProgressLines = new ProgressLines();
var progressLines = view.ProgressLines;

// ορίστε την ημερομηνία από την οποία θα εμφανίζονται οι γραμμές προόδου. Ας ορίσουμε την ημερομηνία κατάστασης του έργου.
progressLines.BeginAtDate = project.Get(Prj.StatusDate);
// ορίστε μια τιμή που υποδεικνύει αν θα εμφανίζονται οι γραμμές προόδου από την αρχή της ημερομηνίας έναρξης του έργου
progressLines.BeginAtProjectStart = true;
// ορίστε τη μορφή ημερομηνίας (<see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" />).
progressLines.DateFormat = DateLabel.DayDddd;
// ορίστε μια τιμή που υποδεικνύει αν θα εμφανίζεται η γραμμή προόδου στην τρέχουσα ημερομηνία.
progressLines.DisplayAtCurrentDate = true;
// ορίστε μια τιμή που υποδεικνύει αν θα εμφανίζεται η γραμμή προόδου σε επαναλαμβανόμενα διαστήματα.
progressLines.DisplayAtRecurringIntervals = true;
// ορίστε μια τιμή που υποδεικνύει αν θα εμφανίζονται οι γραμμές προόδου στις επιλεγμένες ημερομηνίες
progressLines.DisplaySelected = true;
// ορίστε μια τιμή που υποδεικνύει αν θα εμφανίζονται οι γραμμές προόδου για το βασικό σχέδιο ή το πραγματικό.
progressLines.IsBaselinePlan = false;
// ορίστε τη γραμματοσειρά που χρησιμοποιείται για την ετικέτα της γραμμής προόδου.
progressLines.Font = new FontDescriptor("Arial", 10);
// ορίστε το χρώμα γραμμής για την τρέχουσα γραμμή προόδου.
progressLines.LineColor = Color.Aquamarine;
// ορίστε το μοτίβο γραμμής της τρέχουσας γραμμής προόδου.
progressLines.LinePattern = LinePattern.Dashed;
// ορίστε το χρώμα της άλλης γραμμής προόδου.
progressLines.OtherLineColor = Color.Azure;
// ορίστε το μοτίβο γραμμής για την άλλη γραμμή προόδου.
progressLines.OtherLinePattern = LinePattern.Dotted;
// ορίστε το χρώμα του άλλου σημείου προόδου.
progressLines.OtherProgressPointColor = Color.Red;
// ορίστε το σχήμα του σημείου προόδου της άλλης γραμμής προόδου.
progressLines.OtherProgressPointShape = GanttBarEndShape.Circle;
// ορίστε το χρώμα του σημείου προόδου.
progressLines.ProgressPointColor = Color.Orange;
// ορίστε το σχήμα του σημείου προόδου.
progressLines.ProgressPointShape = GanttBarEndShape.Diamond;
// ορίστε το επαναλαμβανόμενο διάστημα.
progressLines.RecurringInterval = new RecurringInterval();
// ορίστε το επαναλαμβανόμενο διάστημα.
progressLines.RecurringInterval.Interval = Interval.Daily;
// ορίστε τον ημερήσιο αριθμό ημέρας
progressLines.RecurringInterval.DailyDayNumber = 1;
// ορίστε μια τιμή που υποδεικνύει αν θα εμφανίζεται η ημερομηνία για κάθε γραμμή προόδου.
progressLines.ShowDate = true;

// ας ελέγξουμε τις γραμμές προόδου
Console.WriteLine("Begin At Date: " + progressLines.BeginAtDate);
Console.WriteLine("Begin At Project Start: " + progressLines.BeginAtProjectStart);
Console.WriteLine("Date Format: " + progressLines.DateFormat);
Console.WriteLine("Display At Current Date: " + progressLines.DisplayAtCurrentDate);
Console.WriteLine("Display At Recurring Intervals: " + progressLines.DisplayAtRecurringIntervals);
Console.WriteLine("Display Selected: " + progressLines.DisplaySelected);
Console.WriteLine("Font: " + progressLines.Font);
Console.WriteLine("Is Baseline Plan: " + progressLines.IsBaselinePlan);
Console.WriteLine("Line Color: " + progressLines.LineColor);
Console.WriteLine("Line Pattern: " + progressLines.LinePattern);
Console.WriteLine("Other Line Color: " + progressLines.OtherLineColor);
Console.WriteLine("Other Line Pattern: " + progressLines.OtherLinePattern);
Console.WriteLine("Other Progress Point Color: " + progressLines.OtherProgressPointColor);
Console.WriteLine("Other Progress Point Shape: " + progressLines.OtherProgressPointShape);
Console.WriteLine("Progress Point Color: " + progressLines.ProgressPointColor);
Console.WriteLine("Progress Point Shape: " + progressLines.ProgressPointShape);
Console.WriteLine("Recurring Interval: " + progressLines.RecurringInterval.Interval);
Console.WriteLine("Recurring Interval DailyDayNumber: " + progressLines.RecurringInterval.DailyDayNumber);
Console.WriteLine("Selected Dates: ");
foreach (var date in progressLines.SelectedDates)
{
    Console.WriteLine("Date: " + date);
}
Console.WriteLine("Show Date: " + progressLines.ShowDate);
Console.WriteLine();

project.Save(OutDir + "WorkWithProgressLines_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [RecurringInterval](../../recurringinterval/)
* class [ProgressLines](../)
* namespace [Aspose.Tasks.Visualization](../../progresslines/)
* assembly [Aspose.Tasks](../../../)


