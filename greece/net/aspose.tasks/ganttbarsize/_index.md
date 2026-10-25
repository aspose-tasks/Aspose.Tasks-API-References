---
title: "Απαρίθμηση GanttBarSize"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.GanttBarSize απαρίθμηση. Καθορίζει το ύψος μιας μπάρας σε σημεία"
type: docs
weight: 700
url: /el/net/aspose.tasks/ganttbarsize/
---
## GanttBarSize enumeration

Καθορίζει το ύψος μιας γραμμής σε σημεία.

```csharp
public enum GanttBarSize
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| BarSize6 | `0` | Μέγεθος μπάρας 6 σημεία. |
| BarSize8 | `1` | Μέγεθος μπάρας 8 σημεία. |
| BarSize10 | `2` | Μέγεθος μπάρας 10 σημεία. |
| BarSize12 | `3` | Μέγεθος μπάρας 12 σημεία. |
| BarSize14 | `4` | Μέγεθος μπάρας 14 σημεία. |
| BarSize18 | `5` | Μέγεθος μπάρας 18 σημεία. |
| BarSize24 | `6` | Μέγεθος μπάρας 24 σημεία. |

## Παραδείγματα

Δείχνει πώς να ορίσετε ορισμένες χρήσιμες ιδιότητες της προβολής διαγράμματος Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// ορίστε μια τιμή που υποδεικνύει εάν οι μπάρες στρογγυλοποιούνται στην πλησιέστερη ημέρα
view.BarRounding = false;
// ορίστε το ύψος, σε σημεία, των μπαρών Gantt στο διάγραμμα Gantt
view.BarSize = GanttBarSize.BarSize24;
// ορίστε μια τιμή που υποδεικνύει εάν οι μπάρες συγκέντρωσης θα κρύβονται κατά την επέκταση της συνοπτικής εργασίας
view.HideRollupBarsWhenSummaryExpanded = true;
// ορίστε το χρώμα μη εργάσιμου χρόνου
view.NonWorkingTimeColor = Color.Azure;
// ορίστε μια τιμή που υποδεικνύει εάν οι μπάρες στο διάγραμμα Gantt πρέπει να συγκεντρωθούν
view.RollUpGanttBars = true;
// ορίστε μια τιμή που υποδεικνύει εάν τα διαχωρισμένα τμήματα εργασίας στο διάγραμμα Gantt πρέπει να εμφανίζονται
view.ShowBarSplits = true;
// ορίστε μια τιμή που υποδεικνύει εάν τα σχέδια στο διάγραμμα Gantt πρέπει να εμφανίζονται
view.ShowDrawings = true;
// ορίστε ένα ποσοστό για τη μείωση ή την αύξηση του διαστήματος μεταξύ των μονάδων στο επίπεδο κλίμακας χρόνου
view.TimescaleSizePercentage = 10;

project.Save(OutDir + "WorkWithGanttChartViews_out.pdf", SaveFileFormat.Pdf);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


