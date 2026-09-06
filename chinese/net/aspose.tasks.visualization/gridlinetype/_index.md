---
title: "枚举 GridlineType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.GridlineType 枚举。网格线的类型"
type: docs
weight: 3110
url: /zh/net/aspose.tasks.visualization/gridlinetype/
---
## GridlineType enumeration

网格线的类型。

```csharp
public enum GridlineType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| GanttRow | `0` | 指示甘特行网格线的类型。 |
| TopTierColumn | `1` | 指示顶层列网格线的类型。 |
| BottomTierColumn | `2` | 指示底层列网格线的类型。 |
| SheetRow | `3` | 指示工作表行网格线的类型。 |
| SheetColumn | `4` | 指示工作表列网格线的类型。 |
| UsageRow | `5` | 指示使用行网格线的类型。 |
| UsageColumn | `6` | 指示使用列网格线的类型。 |
| GanttTitleVertical | `7` | 指示甘特标题垂直网格线的类型。 |
| GanttTitleHorizontal | `8` | 指示甘特标题水平网格线的类型。 |
| BarRows | `9` | 指示条行网格线的类型。 |
| GanttProjectStart | `10` | 指示甘特项目开始网格线的类型。 |
| GanttProjectFinish | `11` | 指示甘特项目结束网格线的类型。 |
| GanttStatusDate | `12` | 指示甘特状态日期网格线类型。 |
| GanttCurrentDate | `13` | 指示甘特当前日期网格线类型。 |
| GanttPageBreaks | `14` | 指示甘特分页断点网格线类型。 |
| MiddleTierColumn | `15` | 指示中间层列网格线的网格线类型。 |

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


