---
title: "Gridline.Pattern"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Gridline 属性。获取或设置网格线的 LinePattern"
type: docs
weight: 40
url: /zh/net/aspose.tasks.visualization/gridline/pattern/
---
## Gridline.Pattern property

获取或设置网格线的 [`LinePattern`](../../linepattern/)。

```csharp
public LinePattern Pattern { get; set; }
```

## 示例

展示如何在保存为可视化格式时使用网格线。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // 设置网格线的类型 (<see cref=\"P:Aspose.Tasks.Visualization.Gridline.GridlineType\" />)。
    GridlineType = GridlineType.GanttRow, 
    // 设置网格线的 <see cref=\"T:Aspose.Tasks.Visualization.LinePattern\" />
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### 另见

* enum [LinePattern](../../linepattern/)
* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


