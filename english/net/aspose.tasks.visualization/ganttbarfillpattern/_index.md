---
title: Enum GanttBarFillPattern
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.GanttBarFillPattern enum. A shapes fill pattern
type: docs
weight: 3010
url: /net/aspose.tasks.visualization/ganttbarfillpattern/
---
## GanttBarFillPattern enumeration

A shape's fill pattern.

```csharp
public enum GanttBarFillPattern
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Hollow | `0` | Hollow pattern. |
| SolidFill | `1` | Solid fill pattern. |
| LightFill | `2` | Light fill pattern. |
| MediumFill | `3` | Medium fill pattern. |
| DarkFill | `4` | Dark fill pattern. |
| DiagonalLeft | `5` | Diagonal left pattern (from the upper left to the lower right). |
| DiagonalRight | `6` | Diagonal right pattern (from the upper right to the lower left). |
| DiagonalCross | `7` | Diagonal cross pattern. |
| LineVertical | `8` | Line vertical pattern. |
| LineHorizontal | `9` | Line horizontal pattern. |
| LineCross | `10` | Line cross pattern. |
| SolidFillWithDashedBorder | `11` | Solid with dashed border pattern. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


