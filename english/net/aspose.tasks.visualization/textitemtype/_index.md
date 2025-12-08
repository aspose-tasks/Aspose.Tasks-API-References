---
title: Enum TextItemType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.TextItemType enum. Item type to change a text style for
type: docs
weight: 3360
url: /net/aspose.tasks.visualization/textitemtype/
---
## TextItemType enumeration

Item type to change a text style for.

```csharp
public enum TextItemType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| RowColumnTitles | `0` | Row and column titles. |
| CriticalTasks | `1` | Critical tasks. |
| NoncriticalTasks | `2` | Noncritical tasks. |
| MilestoneTasks | `3` | Milestone tasks. |
| InactiveTasks | `4` | Inactive tasks. |
| SummaryTasks | `5` | Summary tasks. |
| AssignmentRow | `6` | Assignment row. |
| TopTimescaleTier | `7` | Top timescale tier. |
| BottomTimescaleTier | `8` | Bottom timescale tier. |
| MiddleTimescaleTier | `9` | Middle timescale tier. |
| Resources | `10` | Resource sheet. |
| OverallocatedResources | `11` | Over allocated resources. |
| TaskFilterHighlight | `12` | Task Filter Highlight text item. |
| BarTextBottom | `13` | Bar Text Bottom text item. |
| BarTextInside | `14` | Bar Text Inside text item. |
| BarTextLeft | `15` | Bar Text Left text item. |
| BarTextRight | `16` | Bar Text Right text item. |
| BarTextTop | `17` | Bar Text Top text item. |
| MarkedTasks | `18` | Marked task text item. |
| ProjectSummary | `19` | Project summary task text item. |
| ExternalTasks | `20` | External tasks text item. |
| Allocated | `21` | Allocated text item. |
| ChangedCells | `22` | Changed cells. |

## Examples

Shows how to work with text item types.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Italic | FontStyles.Bold)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


