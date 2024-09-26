---
title: GanttChartView.CustomBarStyles
second_title: Aspose.Tasks for .NET API Reference
description: GanttChartView property. Gets a list of custom taskspecific bar styles of the Gantt Chart view. GanttBarStyle
type: docs
weight: 70
url: /net/aspose.tasks/ganttchartview/custombarstyles/
---
## GanttChartView.CustomBarStyles property

Gets a list of custom task-specific bar styles of the Gantt Chart view. [`GanttBarStyle`](../../../aspose.tasks.visualization/ganttbarstyle/).

```csharp
public List<GanttBarStyle> CustomBarStyles { get; }
```

## Examples

Shows how to set custom bar styles of Gantt Chart project view.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Add the custom bar style to the custom bar collection of the project view
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

### See Also

* class [GanttBarStyle](../../../aspose.tasks.visualization/ganttbarstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


