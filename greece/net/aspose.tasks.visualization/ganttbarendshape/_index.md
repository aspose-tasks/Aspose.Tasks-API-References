---
title: "Απαρίθμηση GanttBarEndShape"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.Visualization.GanttBarEndShape. Αντιπροσωπεύει το σχήμα τέλους σε ράβδους και σημεία προόδου σε γραμμές προόδου"
type: docs
weight: 3030
url: /el/net/aspose.tasks.visualization/ganttbarendshape/
---
## GanttBarEndShape enumeration

Αντιπροσωπεύει το σχήμα τέλους σε μπαρ και σημεία προόδου σε γραμμές προόδου.

```csharp
public enum GanttBarEndShape
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| ArrowDown | `14` | Δείχνει βέλος που δείχνει προς τα κάτω σχήμα τέλους ράβδου Gantt. |
| ArrowUp | `8` | Δείχνει βέλος που δείχνει προς τα πάνω σχήμα τέλους ράβδου Gantt. |
| CaretDownTop | `9` | Δείχνει caret που δείχνει προς τα κάτω στο επάνω μισό της ράβδου σχήμα τέλους Gantt. |
| CaretUpBottom | `10` | Δείχνει caret που δείχνει προς τα πάνω στο κάτω μισό της ράβδου σχήμα τέλους Gantt. |
| Circle | `19` | Δείχνει κύκλο σχήμα τέλους ράβδου Gantt. |
| CircleArrowDown | `18` | Δείχνει βέλος σε κύκλο που δείχνει προς τα κάτω σχήμα τέλους ράβδου Gantt. |
| CircleArrowUp | `17` | Δείχνει βέλος σε κύκλο που δείχνει προς τα πάνω σχήμα τέλους ράβδου Gantt. |
| CircleDiamond | `13` | Δείχνει διαμάντι σε κύκλο σχήμα τέλους ράβδου Gantt. |
| CircleTriangleDown | `16` | Δείχνει τρίγωνο σε κύκλο που δείχνει προς τα κάτω σχήμα τέλους ράβδου Gantt. |
| CircleTriangleUp | `15` | Δείχνει τρίγωνο σε κύκλο που δείχνει προς τα πάνω σχήμα τέλους ράβδου Gantt. |
| Diamond | `3` | Δείχνει διαμάντι σχήμα τέλους ράβδου Gantt. |
| HouseDown | `2` | Δείχνει σπίτι ανάποδα σχήμα τέλους ράβδου Gantt. |
| HouseUp | `1` | Δείχνει σπίτι σχήμα τέλους ράβδου Gantt. |
| LeftBracket | `21` | Δείχνει αριστερή αγκύλη σχήμα τέλους ράβδου Gantt. |
| LeftFade | `23` | Δείχνει αριστερό ξεθώριασμα σχήμα τέλους ράβδου Gantt. |
| LineShape | `11` | Δείχνει γραμμή σχήμα τέλους ράβδου Gantt. |
| NoBarEndShape | `0` | Δείχνει κανένα σχήμα τέλους ράβδου Gantt. |
| RightBracket | `22` | Δείχνει δεξιά αγκύλη σχήμα τέλους ράβδου Gantt. |
| RightFade | `24` | Δείχνει δεξιό ξεθώριασμα σχήμα τέλους ράβδου Gantt. |
| Square | `12` | Δείχνει τετράγωνο σχήμα τέλους ράβδου Gantt. |
| Star | `20` | Δείχνει αστέρι σχήμα τέλους ράβδου Gantt. |
| TriangleDown | `5` | Δείχνει τρίγωνο που δείχνει προς τα κάτω σχήμα τέλους ράβδου Gantt. |
| TriangleLeft | `7` | Δείχνει το σχήμα τριγώνου που δείχνει αριστερά στο άκρο της μπάρας Gantt. |
| TriangleRight | `6` | Δείχνει το σχήμα τριγώνου που δείχνει δεξιά στο άκρο της μπάρας Gantt. |
| TriangleUp | `4` | Δείχνει τρίγωνο σε κύκλο που δείχνει προς τα πάνω σχήμα τέλους ράβδου Gantt. |

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


