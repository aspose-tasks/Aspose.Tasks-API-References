---
title: "类 Gridline"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.Gridline 类。出现在项目视图中的水平或垂直线"
type: docs
weight: 3100
url: /zh/net/aspose.tasks.visualization/gridline/
---
## Gridline class

出现在项目视图中的水平或垂直线。

```csharp
public class Gridline
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Gridline](gridline/)() | 初始化 `Gridline` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Color](../../aspose.tasks.visualization/gridline/color/) { get; set; } | 获取或设置网格线的 [`Color`](./color/)。 |
| [GridlineType](../../aspose.tasks.visualization/gridline/gridlinetype/) { get; set; } | 获取或设置网格线的类型（[`GridlineType`](./gridlinetype/)）。 |
| [Pattern](../../aspose.tasks.visualization/gridline/pattern/) { get; set; } | 获取或设置网格线的 [`LinePattern`](../linepattern/)。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Equals](../../aspose.tasks.visualization/gridline/equals/)(object) | 返回一个标志，指示此实例是否等于指定的对象。 |
| override [GetHashCode](../../aspose.tasks.visualization/gridline/gethashcode/)() | 返回 `Gridline` 类实例的哈希码值。 |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


