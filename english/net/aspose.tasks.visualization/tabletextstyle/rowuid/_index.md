---
title: TableTextStyle.RowUid
second_title: Aspose.Tasks for .NET API Reference
description: TableTextStyle property. Gets a row unique id. Return 1 if the style is to be applied to all rows of a view
type: docs
weight: 40
url: /net/aspose.tasks.visualization/tabletextstyle/rowuid/
---
## TableTextStyle.RowUid property

Gets a row unique id. Return -1 if the style is to be applied to all rows of a view.

```csharp
public int RowUid { get; }
```

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

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


