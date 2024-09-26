---
title: GanttChartView.TableTextStyles
second_title: Aspose.Tasks for .NET API Reference
description: GanttChartView property. Gets a list of table text styles of the Gantt Chart view. TableTextStyle
type: docs
weight: 160
url: /net/aspose.tasks/ganttchartview/tabletextstyles/
---
## GanttChartView.TableTextStyles property

Gets a list of table text styles of the Gantt Chart view. [`TableTextStyle`](../../../aspose.tasks.visualization/tabletextstyle/).

```csharp
public List<TableTextStyle> TableTextStyles { get; }
```

## Examples

Shows how to add custom table text styles.

```csharp
var project = new Project(DataDir + "Project5.mpp");
var view = (GanttChartView)project.Views.ToList()[0];

view.TableTextStyles.Clear();
view.TableTextStyles.Add(new TableTextStyle(1) { Color = Color.Red, Field = Field.TaskName });
view.TableTextStyles.Add(new TableTextStyle(1) { Color = Color.Gray, Field = Field.TaskDurationText });
view.TableTextStyles.Add(new TableTextStyle(2, FontStyles.Bold | FontStyles.Italic | FontStyles.Underline)
{
    Color = Color.Blue
});
```

### See Also

* class [TableTextStyle](../../../aspose.tasks.visualization/tabletextstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


