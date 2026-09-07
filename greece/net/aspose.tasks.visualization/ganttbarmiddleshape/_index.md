---
title: "Απαρίθμηση GanttBarMiddleShape"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.Visualization.GanttBarMiddleShape. Καθορίζει το μεσαίο σχήμα μιας μπάρας."
type: docs
weight: 3050
url: /el/net/aspose.tasks.visualization/ganttbarmiddleshape/
---
## GanttBarMiddleShape enumeration

Καθορίζει το μεσαίο σχήμα μιας μπάρας.

```csharp
public enum GanttBarMiddleShape
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| LineBottom | `7` | Δείχνει σχήμα γραμμής με στοίχιση στο κάτω μέρος. |
| LineMiddle | `6` | Δείχνει σχήμα γραμμής με κεντρική στοίχιση. |
| LineTop | `5` | Δείχνει σχήμα γραμμής με στοίχιση στην κορυφή. |
| None | `0` | Δείχνει κενό σχήμα. |
| RectangleBar | `1` | Δείχνει σχήμα ορθογωνίου μπάρας πλήρους ύψους. |
| RectangleBottom | `4` | Δείχνει σχήμα ορθογωνίου μπάρας μισού ύψους ευθυγραμμισμένο στο κάτω μέρος. |
| RectangleMiddle | `3` | Δείχνει σχήμα ορθογωνίου μπάρας 1/3 ύψους ευθυγραμμισμένο στο κέντρο. |
| RectangleTop | `2` | Δείχνει σχήμα ορθογωνίου ράβδου μισού ύψους με στοίχιση στην κορυφή. |

## Παραδείγματα

Δείχνει πώς να ορίσετε προσαρμοσμένα στυλ μπάρας στην προβολή έργου Gantt Chart.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Προσθέστε το προσαρμοσμένο στυλ μπάρας στη συλλογή προσαρμοσμένων μπαρών της προβολής έργου
        view.CustomBarStyles.Add(custom);

        SimpleSaveOptions options = new MPPSaveOptions
        {
            WriteViewData = true
        };

        project.Save(OutDir + "ImplementCustomBarStyleWriting_out.mpp", options);
    }
    catch (NotSupportedException ex)
    {
        Console.WriteLine(
            ex.Message
            + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
    }
}

public static GanttBarStyle GetCustomBarStyle()
{
    var style = new GanttBarStyle
    {
        ShowForTaskUid = 1,
        MiddleShape = GanttBarMiddleShape.RectangleBottom,
        MiddleFillPattern = GanttBarFillPattern.MediumFill,
        MiddleShapeColor = Color.Blue,

        StartShape = GanttBarEndShape.ArrowDown,
        StartShapeColor = Color.Red,

        EndShape = GanttBarEndShape.ArrowUp,
        EndShapeColor = Color.Yellow,

        LeftField = Field.TaskResourceNames,
        RightField = Field.TaskName,
        TopField = Field.TaskStart,
        BottomField = Field.TaskFinish,
        InsideField = Field.TaskDuration
    };

    return style;
}
```

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


