---
title: "Gridline.Gridline"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Gridline 构造函数。初始化 Gridline 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.visualization/gridline/gridline/
---
## Gridline constructor

初始化 [`Gridline`](../) 类的新实例。

```csharp
public Gridline()
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

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


