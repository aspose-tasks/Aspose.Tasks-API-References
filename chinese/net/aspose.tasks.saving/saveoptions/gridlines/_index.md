---
title: "SaveOptions.Gridlines"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SaveOptions 属性。获取或设置在项目视图中出现的 Gridline 列表"
type: docs
weight: 60
url: /zh/net/aspose.tasks.saving/saveoptions/gridlines/
---
## SaveOptions.Gridlines property

获取或设置在项目视图中出现的 [`Gridline`](../../../aspose.tasks.visualization/gridline/) 列表。

```csharp
public List<Gridline> Gridlines { get; set; }
```

## 示例

展示如何将布局保存为单独的文件。

```csharp
var project = new Project(DataDir + "Homemoveplan.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);
options.StartDate = project.Get(Prj.StartDate).AddDays(-3);
options.EndDate = project.Get(Prj.FinishDate);
options.MarkCriticalTasks = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.FontSettings.DefaultFontName = "Segoe UI Black";
options.FontSettings.UseProjectDefaultFont = false;
options.PageSize = PageSize.Letter;

options.Gridlines = new List<Gridline>();

var gridline = new Gridline { GridlineType = GridlineType.GanttRow, Color = Color.CornflowerBlue, Pattern = LinePattern.Dashed };
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles1_out.png", options);

// 将项目布局保存为单独的文件
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### 另见

* class [Gridline](../../../aspose.tasks.visualization/gridline/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


