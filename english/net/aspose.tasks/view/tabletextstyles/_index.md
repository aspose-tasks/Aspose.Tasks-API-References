---
title: View.TableTextStyles
second_title: Aspose.Tasks for .NET API Reference
description: View property. Gets a list of table text styles of the view. TableTextStyle
type: docs
weight: 110
url: /net/aspose.tasks/view/tabletextstyles/
---
## View.TableTextStyles property

Gets a list of table text styles of the view. [`TableTextStyle`](../../../aspose.tasks.visualization/tabletextstyle/).

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
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


