---
title: GanttChartView.TextStyles
second_title: Aspose.Tasks for .NET API Reference
description: GanttChartView property. Gets or sets a list of TextStyle of the Gantt Chart view
type: docs
weight: 170
url: /net/aspose.tasks/ganttchartview/textstyles/
---
## GanttChartView.TextStyles property

Gets or sets a list of [`TextStyle`](../../../aspose.tasks.visualization/textstyle/) of the Gantt Chart view.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Examples

Shows how to read Gantt chart text styles.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// iterate over text styles of the Gantt chart view
foreach (var style in view.TextStyles)
{
    Console.WriteLine("Style Item Type: " + style.ItemType);
    Console.WriteLine("Style Font name: " + style.Font.FontFamily);
    Console.WriteLine();
}
```

### See Also

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


