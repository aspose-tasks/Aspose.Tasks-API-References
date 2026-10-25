---
title: "GanttChartView.BarSize"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "GanttChartView ιδιότητα. Λαμβάνει ή ορίζει το ύψος σε σημεία των ράβδων Gantt στο Gantt Chart"
type: docs
weight: 40
url: /el/net/aspose.tasks/ganttchartview/barsize/
---
## GanttChartView.BarSize property

Λαμβάνει ή ορίζει το ύψος, σε σημεία, των ράβδων Gantt στο Gantt Chart.

```csharp
public GanttBarSize BarSize { get; set; }
```

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

* enum [GanttBarSize](../../ganttbarsize/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


