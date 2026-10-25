---
title: "GanttChartView.TextStyles"
second_title: "Aspose.Tasks for .NET API 参考"
description: "GanttChartView 属性。获取或设置甘特图视图的 TextStyle 列表"
type: docs
weight: 170
url: /zh/net/aspose.tasks/ganttchartview/textstyles/
---
## GanttChartView.TextStyles property

获取或设置甘特图视图的 [`TextStyle`](../../../aspose.tasks.visualization/textstyle/) 列表。

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## 示例

展示如何读取甘特图文本样式。

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// 遍历甘特图视图的文本样式
foreach (var style in view.TextStyles)
{
    Console.WriteLine("Style Item Type: " + style.ItemType);
    Console.WriteLine("Style Font name: " + style.Font.FontFamily);
    Console.WriteLine();
}
```

### 另见

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


