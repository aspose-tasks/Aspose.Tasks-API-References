---
title: "GanttChartView.Gridlines"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα GanttChartView. Λαμβάνει ή ορίζει μια λίστα από Gridlines της προβολής Gantt Chart."
type: docs
weight: 80
url: /el/net/aspose.tasks/ganttchartview/gridlines/
---
## GanttChartView.Gridlines property

Λαμβάνει ή ορίζει μια λίστα από `Gridlines` της προβολής Gantt Chart.

```csharp
public List<Gridlines> Gridlines { get; set; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τις γραμμές πλέγματος.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var view = (GanttChartView)project.Views.ToList()[0];

// επιτρέπει τη ρύθμιση της πρώτης γραμμής πλέγματος της προβολής
var gridlines = view.Gridlines[0];
// ορίστε τον αριθμό από 0 έως 99 που καθορίζει το διάστημα μεταξύ των γραμμών πλέγματος.
gridlines.Interval = 2;
// ορίστε το χρώμα των δευτερευουσών γραμμών πλέγματος.
gridlines.IntervalColor = Color.Red;
// ορίστε το μοτίβο γραμμής για δευτερεύουσες γραμμές πλέγματος
gridlines.IntervalPattern = LinePattern.Solid;
// ορίστε το χρώμα των κανονικών γραμμών πλέγματος
gridlines.NormalColor = Color.Blue;
// ορίστε το μοτίβο γραμμής για κανονικές γραμμές πλέγματος
gridlines.NormalPattern = LinePattern.CloseDot;
// ορίστε τον τύπο της γραμμής πλέγματος
gridlines.Type = GridlineType.GanttRow;

project.Save(OutDir + "WorkWithGridlines_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [Gridlines](../../../aspose.tasks.visualization/gridlines/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


