---
title: "GanttChartView.TableTextStyles"
second_title: "Aspose.Tasks for .NET API 参考"
description: "GanttChartView 属性。获取甘特图视图的表格文本样式列表。TableTextStyle"
type: docs
weight: 160
url: /zh/net/aspose.tasks/ganttchartview/tabletextstyles/
---
## GanttChartView.TableTextStyles property

获取甘特图视图的表格文本样式列表。[`TableTextStyle`](../../../aspose.tasks.visualization/tabletextstyle/)。

```csharp
public List<TableTextStyle> TableTextStyles { get; }
```

## 示例

展示如何添加自定义表格文本样式。

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

### 另见

* class [TableTextStyle](../../../aspose.tasks.visualization/tabletextstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


