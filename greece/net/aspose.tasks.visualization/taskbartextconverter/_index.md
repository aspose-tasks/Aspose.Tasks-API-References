---
title: "Αντιπρόσωπος TaskBarTextConverter"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Προσαρμοσμένος μετατροπέας δεδομένων εργασιών σε κείμενο μπάρας."
type: docs
weight: 3380
url: /el/net/aspose.tasks.visualization/taskbartextconverter/
---
## TaskBarTextConverter delegate

Προσαρμοσμένος μετατροπέας δεδομένων εργασίας σε κείμενο μπάρας.

```csharp
public delegate string TaskBarTextConverter(Task task);
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| εργασία | Εργασία | Εργασία για την οποία θα αποδοθεί το κείμενο της μπάρας εργασίας. |

### Τιμή Επιστροφής

Κείμενο για απόδοση σε μπάρα που αντιστοιχεί στην καθορισμένη εργασία.

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

* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


