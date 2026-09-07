---
title: "Κλάση Gridlines"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.Gridlines class. Αντιπροσωπεύει τις γραμμές πλέγματος που εμφανίζονται σε προβολή GanttChart"
type: docs
weight: 3120
url: /el/net/aspose.tasks.visualization/gridlines/
---
## Gridlines class

Αναπαριστά τις γραμμές πλέγματος που εμφανίζονται σε προβολή GanttChart.

```csharp
public class Gridlines
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Gridlines](gridlines/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Interval](../../aspose.tasks.visualization/gridlines/interval/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό από 0 έως 99 που καθορίζει το διάστημα μεταξύ των γραμμών πλέγματος. |
| [IntervalColor](../../aspose.tasks.visualization/gridlines/intervalcolor/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα των δευτερευουσών γραμμών πλέγματος. |
| [IntervalPattern](../../aspose.tasks.visualization/gridlines/intervalpattern/) { get; set; } | Λαμβάνει ή ορίζει το μοτίβο γραμμής για δευτερεύουσες γραμμές πλέγματος. |
| [NormalColor](../../aspose.tasks.visualization/gridlines/normalcolor/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα των κανονικών γραμμών πλέγματος. |
| [NormalPattern](../../aspose.tasks.visualization/gridlines/normalpattern/) { get; set; } | Λαμβάνει ή ορίζει το μοτίβο γραμμής για κανονικές γραμμές πλέγματος. |
| [Type](../../aspose.tasks.visualization/gridlines/type/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο της γραμμής πλέγματος. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


