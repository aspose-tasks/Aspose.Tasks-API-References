---
title: Enum BarShape
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.BarShape enum. Shape of a bar rectangle
type: docs
weight: 2920
url: /net/aspose.tasks.visualization/barshape/
---
## BarShape enumeration

Shape of a bar rectangle.

```csharp
public enum BarShape
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Full | `0` | Indicates Full rectangle bar shape. |
| HalfHeight | `1` | Indicates top-aligned half height rectangle bar shape. |
| HalfHeightBottom | `2` | Indicates bottom-aligned half height rectangle bar shape. |
| Thin | `3` | Indicates center-aligned line shape. |
| None | `4` | Indicates None bar shape. |
| Middle | `5` | Indicates center-aligned line shape. |
| LineBottom | `6` | Indicates bottom-aligned line shape. |
| LineTop | `7` | Indicates top-aligned line shape. |

## Examples

Shows how to use custom bar styles.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    BarStyles = new List<BarStyle>()
};

// add a bar style for milestone tasks
var style = new BarStyle();
// set <see cref="T:Aspose.Tasks.Visualization.BarItemType" /> of the bar style
style.ItemType = BarItemType.Milestone;
// set <see cref="T:System.Drawing.Color" /> of the bar style.
style.BarColor = Color.Green;
// set <see cref="P:Aspose.Tasks.Visualization.BarStyle.BarShape" /> of the bar style
style.BarShape = BarShape.HalfHeight;
// set <see cref="T:Aspose.Tasks.Visualization.Shape" /> at the beginning of the bar
style.StartShape = Shape.LeftBracket;
// set <see cref="T:System.Drawing.Color" /> of the shape at the beginning of the bar
style.StartShapeColor = Color.Aqua;
// set <see cref="T:Aspose.Tasks.Visualization.Shape" /> at the end of the bar
style.EndShape = Shape.RightBracket;
// set <see cref="T:System.Drawing.Color" /> of the shape at the end of the bar
style.EndShapeColor = Color.Aquamarine;
// set of the text to render on the right of the bar.
style.TextStyle = new TextStyle();
style.TextStyle.BackgroundColor = Color.Black;

// there is exists a feature that allow to convert a text of the bar
// lets set converter to get text for the bar to render.
style.LeftBarTextConverter = task =>
{
    if (!task.Get(Tsk.Name).StartsWith("T"))
    {
        task.Set(Tsk.Name, "T" + task.Get(Tsk.Name));
    }

    return task.Get(Tsk.Name);
};

options.BarStyles.Add(style);

// save the project
project.Save(OutDir + "WorkWithBarStyle_out.mpp", options);
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


