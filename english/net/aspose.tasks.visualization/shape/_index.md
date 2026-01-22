---
title: Enum Shape
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.Shape enum. Shape of a marker at the beginning or end of the bar style to be rendered when saving view data to some of SaveFileFormat
type: docs
weight: 3330
url: /net/aspose.tasks.visualization/shape/
---
## Shape enumeration

Shape of a marker at the beginning or end of the bar style to be rendered when saving view data to some of [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/).

```csharp
public enum Shape
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Indicates None shape. |
| VerticalLine | `1` | Indicates Vertical line shape. |
| Pentagon | `2` | Indicates Pentagon shape. |
| Triangle | `3` | Indicates Triangle shape. |
| LeftBracket | `4` | Indicates Left bracket shape. |
| RightBracket | `5` | Indicates Right bracket shape. |
| ArrowDown | `6` | Indicates ArrowDown shape. |
| LeftFade | `7` | Indicates Left fade shape. |
| RightFade | `8` | Indicates Right fade shape. |
| Diamond | `9` | Indicates Diamond shape. |
| Circle | `10` | Indicates Circle shape. |

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


