---
title: Class TableTextStyle
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.TableTextStyle class. Represents a text style in a view table
type: docs
weight: 3350
url: /net/aspose.tasks.visualization/tabletextstyle/
---
## TableTextStyle class

Represents a text style in a view table.

```csharp
public class TableTextStyle : TextStyle
```

## Constructors

| Name | Description |
| --- | --- |
| [TableTextStyle](tabletextstyle/#constructor)(int) | Initializes a new instance of the `TableTextStyle` class. |
| [TableTextStyle](tabletextstyle/#constructor_1)(int, FontDescriptor) | Initializes a new instance of the `TableTextStyle` class with the specified font. |
| [TableTextStyle](tabletextstyle/#constructor_2)(int, FontStyles) | Initializes a new instance of the `TableTextStyle` class with the default font settings and the specified font style. |
| [TableTextStyle](tabletextstyle/#constructor_3)(int, float, FontStyles) | Initializes a new instance of the `TableTextStyle` class with the specified font size and font style. |

## Properties

| Name | Description |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Gets or sets background color of the text style. [`Color`](../textstyle/color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Gets or sets background pattern of the text style. [`BackgroundPattern`](../textstyle/backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Gets or sets color of the text. |
| [Field](../../aspose.tasks.visualization/tabletextstyle/field/) { get; set; } | Gets or sets a field the style is to be applied to. [`Field`](./field/). |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Gets or sets font of the text style. |
| override [ItemType](../../aspose.tasks.visualization/tabletextstyle/itemtype/) { get; } | Returns a value of the [`TextItemType`](../textitemtype/) enum. |
| [RowUid](../../aspose.tasks.visualization/tabletextstyle/rowuid/) { get; } | Gets a row unique id. Return -1 if the style is to be applied to all rows of a view. |

## Examples

Shows how to customize table text styles which are used to style different text items in a project.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// set first task name text style
var style1 = new TableTextStyle(1);
// set a field the style is to be applied to.
style1.Field = Field.TaskName;
// set <see cref="P:Aspose.Tasks.Visualization.TextStyle.Font" /> of the text style.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// set size in points of the text style font.

// set second task duration text style
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // set a flag indicating that view data must be written
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### See Also

* class [TextStyle](../textstyle/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


