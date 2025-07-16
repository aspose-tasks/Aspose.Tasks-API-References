---
title: Class BarStyle
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.BarStyle class. Change the visual style of the bar for the item in the project view
type: docs
weight: 2880
url: /net/aspose.tasks.visualization/barstyle/
---
## BarStyle class

Change the visual style of the bar for the item in the project view.

```csharp
public class BarStyle
```

## Constructors

| Name | Description |
| --- | --- |
| [BarStyle](barstyle/)() | Initializes a new instance of the `BarStyle` class. |

## Properties

| Name | Description |
| --- | --- |
| [BarColor](../../aspose.tasks.visualization/barstyle/barcolor/) { get; set; } | Gets or sets Color of the bar style. |
| [BarShape](../../aspose.tasks.visualization/barstyle/barshape/) { get; set; } | Gets or sets [`BarShape`](./barshape/) of the bar style. |
| [BottomBarTextConverter](../../aspose.tasks.visualization/barstyle/bottombartextconverter/) { get; set; } | Gets or sets user-defined converter to get text to render on the bottom of the task's bar. Overrides the value of [`BottomField`](./bottomfield/) property. |
| [BottomField](../../aspose.tasks.visualization/barstyle/bottomfield/) { get; set; } | Gets or sets a field to be displayed on the bottom of the bar. |
| [EndShape](../../aspose.tasks.visualization/barstyle/endshape/) { get; set; } | Gets or sets [`Shape`](../shape/) at the end of the bar. |
| [EndShapeColor](../../aspose.tasks.visualization/barstyle/endshapecolor/) { get; set; } | Gets or sets Color of the shape at the end of the bar. |
| [EndShapeType](../../aspose.tasks.visualization/barstyle/endshapetype/) { get; set; } | Gets or sets a type of the end shape. [`GanttBarType`](../ganttbartype/). |
| [From](../../aspose.tasks.visualization/barstyle/from/) { get; set; } | Gets or sets a start point position of the gantt bar. [`Field`](../../aspose.tasks/field/). |
| [InsideBarTextConverter](../../aspose.tasks.visualization/barstyle/insidebartextconverter/) { get; set; } | Gets or sets user-defined converter to get text to render inside of the task's bar. Overrides the value of [`InsideField`](./insidefield/) property. |
| [InsideField](../../aspose.tasks.visualization/barstyle/insidefield/) { get; set; } | Gets or sets a field to be displayed inside of the bar. |
| [ItemType](../../aspose.tasks.visualization/barstyle/itemtype/) { get; set; } | Gets or sets [`BarItemType`](../baritemtype/) of the bar style. |
| [LeftBarTextConverter](../../aspose.tasks.visualization/barstyle/leftbartextconverter/) { get; set; } | Gets or sets user-defined converter to get text to render on the left of the task's bar. Overrides the value of [`LeftField`](./leftfield/) property. |
| [LeftField](../../aspose.tasks.visualization/barstyle/leftfield/) { get; set; } | Gets or sets a field to be displayed on the left of the bar. |
| [RightBarTextConverter](../../aspose.tasks.visualization/barstyle/rightbartextconverter/) { get; set; } | Gets or sets user-defined converter to get text to render on the right of the task's bar. Overrides the value of [`RightField`](./rightfield/) property. |
| [RightField](../../aspose.tasks.visualization/barstyle/rightfield/) { get; set; } | Gets or sets a field to be displayed on the right of the bar. |
| [StartShape](../../aspose.tasks.visualization/barstyle/startshape/) { get; set; } | Gets or sets [`Shape`](../shape/) at the beginning of the bar. |
| [StartShapeColor](../../aspose.tasks.visualization/barstyle/startshapecolor/) { get; set; } | Gets or sets Color of the shape at the beginning of the bar. |
| [StartShapeType](../../aspose.tasks.visualization/barstyle/startshapetype/) { get; set; } | Gets or sets a type of the start shape. |
| [TextStyle](../../aspose.tasks.visualization/barstyle/textstyle/) { get; set; } | Gets or sets style of the bar's text. |
| [To](../../aspose.tasks.visualization/barstyle/to/) { get; set; } | Gets or sets a finish point position of the gantt bar. |
| [TopBarTextConverter](../../aspose.tasks.visualization/barstyle/topbartextconverter/) { get; set; } | Gets or sets user-defined converter to get text to render on the top of the task's bar. Overrides the value of [`TopField`](./topfield/) property. |
| [TopField](../../aspose.tasks.visualization/barstyle/topfield/) { get; set; } | Gets or sets a field to be displayed on the top of the bar. |

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


