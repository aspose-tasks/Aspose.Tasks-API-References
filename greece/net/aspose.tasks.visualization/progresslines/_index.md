---
title: "Κλάση ProgressLines"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Visualization.ProgressLines. Αντιπροσωπεύει τις γραμμές προόδου σε προβολή διαγράμματος Gantt"
type: docs
weight: 3290
url: /el/net/aspose.tasks.visualization/progresslines/
---
## ProgressLines class

Αναπαριστά τις γραμμές προόδου σε προβολή Gantt Chart.

```csharp
public class ProgressLines
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ProgressLines](progresslines/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [BeginAtDate](../../aspose.tasks.visualization/progresslines/beginatdate/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία από την οποία θα εμφανίζονται οι γραμμές προόδου. |
| [BeginAtProjectStart](../../aspose.tasks.visualization/progresslines/beginatprojectstart/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται οι γραμμές προόδου από την αρχή της ημερομηνίας έναρξης του έργου. |
| [DateFormat](../../aspose.tasks.visualization/progresslines/dateformat/) { get; set; } | Λαμβάνει ή ορίζει τη μορφή ημερομηνίας ([`DateLabel`](../datelabel/)). |
| [DisplayAtCurrentDate](../../aspose.tasks.visualization/progresslines/displayatcurrentdate/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζεται η γραμμή προόδου στην τρέχουσα ημερομηνία. |
| [DisplayAtRecurringIntervals](../../aspose.tasks.visualization/progresslines/displayatrecurringintervals/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζεται η γραμμή προόδου σε επαναλαμβανόμενα διαστήματα. |
| [DisplaySelected](../../aspose.tasks.visualization/progresslines/displayselected/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται οι γραμμές προόδου στις επιλεγμένες ημερομηνίες. |
| [Font](../../aspose.tasks.visualization/progresslines/font/) { get; set; } | Λαμβάνει ή ορίζει τη γραμματοσειρά που χρησιμοποιείται για την ετικέτα της γραμμής προόδου. |
| [IsBaselinePlan](../../aspose.tasks.visualization/progresslines/isbaselineplan/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται οι γραμμές προόδου για το βασικό σχέδιο ή το πραγματικό. |
| [LineColor](../../aspose.tasks.visualization/progresslines/linecolor/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα της γραμμής για την τρέχουσα γραμμή προόδου. |
| [LinePattern](../../aspose.tasks.visualization/progresslines/linepattern/) { get; set; } | Λαμβάνει ή ορίζει το μοτίβο γραμμής της τρέχουσας γραμμής προόδου. [`LinePattern`](./linepattern/). |
| [OtherLineColor](../../aspose.tasks.visualization/progresslines/otherlinecolor/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα της άλλης γραμμής προόδου. |
| [OtherLinePattern](../../aspose.tasks.visualization/progresslines/otherlinepattern/) { get; set; } | Λαμβάνει ή ορίζει το μοτίβο γραμμής για την άλλη γραμμή προόδου. |
| [OtherProgressPointColor](../../aspose.tasks.visualization/progresslines/otherprogresspointcolor/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα του άλλου σημείου προόδου. |
| [OtherProgressPointShape](../../aspose.tasks.visualization/progresslines/otherprogresspointshape/) { get; set; } | Λαμβάνει ή ορίζει το σχήμα του σημείου προόδου της άλλης γραμμής προόδου. |
| [ProgressPointColor](../../aspose.tasks.visualization/progresslines/progresspointcolor/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα του σημείου προόδου. |
| [ProgressPointShape](../../aspose.tasks.visualization/progresslines/progresspointshape/) { get; set; } | Λαμβάνει ή ορίζει το σχήμα του σημείου προόδου. [`GanttBarEndShape`](../ganttbarendshape/). |
| [RecurringInterval](../../aspose.tasks.visualization/progresslines/recurringinterval/) { get; set; } | Λαμβάνει ή ορίζει το επαναλαμβανόμενο διάστημα. [`RecurringInterval`](./recurringinterval/). |
| [SelectedDates](../../aspose.tasks.visualization/progresslines/selecteddates/) { get; } | Λαμβάνει τη λίστα των επιλεγμένων ημερομηνιών για τις οποίες θα εμφανιστούν γραμμές προόδου. |
| [ShowDate](../../aspose.tasks.visualization/progresslines/showdate/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζεται η ημερομηνία για κάθε γραμμή προόδου. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


