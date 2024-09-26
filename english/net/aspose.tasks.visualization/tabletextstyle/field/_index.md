---
title: TableTextStyle.Field
second_title: Aspose.Tasks for .NET API Reference
description: TableTextStyle property. Gets or sets a field the style is to be applied to. Field
type: docs
weight: 20
url: /net/aspose.tasks.visualization/tabletextstyle/field/
---
## TableTextStyle.Field property

Gets or sets a field the style is to be applied to. `Field`.

```csharp
public Field Field { get; set; }
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

* enum [Field](../../../aspose.tasks/field/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


