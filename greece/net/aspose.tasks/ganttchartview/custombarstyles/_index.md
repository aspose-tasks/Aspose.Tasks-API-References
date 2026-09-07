---
title: "GanttChartView.CustomBarStyles"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "GanttChartView ιδιότητα. Λαμβάνει μια λίστα με προσαρμοσμένα στυλ ράβδων ειδικά για εργασίες της προβολής Gantt Chart. GanttBarStyle"
type: docs
weight: 70
url: /el/net/aspose.tasks/ganttchartview/custombarstyles/
---
## GanttChartView.CustomBarStyles property

Λαμβάνει μια λίστα με προσαρμοσμένα στυλ ράβδων ειδικά για εργασίες της προβολής Gantt Chart. [`GanttBarStyle`](../../../aspose.tasks.visualization/ganttbarstyle/).

```csharp
public List<GanttBarStyle> CustomBarStyles { get; }
```

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

### Δείτε επίσης

* class [GanttBarStyle](../../../aspose.tasks.visualization/ganttbarstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


