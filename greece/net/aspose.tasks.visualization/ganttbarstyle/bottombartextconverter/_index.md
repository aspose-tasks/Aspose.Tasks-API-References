---
title: "GanttBarStyle.BottomBarTextConverter"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "GanttBarStyle ιδιότητα. Λαμβάνει ή ορίζει προσαρμοσμένο μετατροπέα για λήψη κειμένου που θα αποδοθεί στο κάτω μέρος της γραμμής των εργασιών. Αντικαθιστά την τιμή της ιδιότητας BottomField"
type: docs
weight: 20
url: /el/net/aspose.tasks.visualization/ganttbarstyle/bottombartextconverter/
---
## GanttBarStyle.BottomBarTextConverter property

Λαμβάνει ή ορίζει μετατροπέα που ορίζεται από τον χρήστη για λήψη κειμένου που θα αποδοθεί στο κάτω μέρος της γραμμής της εργασίας. Αντικαθιστά την τιμή της ιδιότητας [`BottomField`](../bottomfield/).

```csharp
public TaskBarTextConverter BottomBarTextConverter { get; set; }
```

## Παρατηρήσεις

Δεν αποθηκεύεται σε μορφή MPP.

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε προσαρμοσμένα στυλ μπάρας στην προβολή Gantt Chart.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// Τα στυλ μπάρας μπορούν να είναι είτε ειδικά για εργασία (βρίσκονται στο GanttChartView.CustomBarStyles)
// ή ειδικά για κατηγορία (βρίσκονται στο GanttChartView.BarStyles)
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // Για σκοπούς επίδειξης, τροποποιούμε το στυλ για εργασία με μοναδικό αναγνωριστικό = 4
    // Εδώ ορίζουμε το πεδίο (TaskName) ώστε να αποδίδεται στα αριστερά της μπάρας εργασίας.
    ganttBarStyle.LeftField = Field.TaskName;
    // Εδώ ορίζουμε προσαρμοσμένο μετατροπέα για να ελέγξουμε ποιο κείμενο θα αποδίδεται μέσα στη μπάρα εργασίας.
    ganttBarStyle.InsideBarTextConverter = task => "Hours rem.: " + (int)task.Get(Tsk.RemainingWork).TimeSpan.TotalHours;

    ganttBarStyle.MiddleShapeColor = Color.Green;
    ganttBarStyle.MiddleShape = GanttBarMiddleShape.LineTop;
    ganttBarStyle.StartShape = GanttBarEndShape.LeftBracket;
    ganttBarStyle.StartShapeColor = Color.Aqua;
    ganttBarStyle.EndShape = GanttBarEndShape.RightBracket;
    ganttBarStyle.EndShapeColor = Color.Aquamarine;
}

foreach (GanttBarStyle ganttBarStyle in ganttChartView.BarStyles)
{
    if (!ganttBarStyle.ShowForCategories.Contains(GanttBarShowFor.Milestone))
    {
        continue;
    }

    // Για σκοπούς επίδειξης, τροποποιούμε τα στυλ που ισχύουν για εργασίες ορόσημου.

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

### Δείτε επίσης

* delegate [TaskBarTextConverter](../../taskbartextconverter/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


