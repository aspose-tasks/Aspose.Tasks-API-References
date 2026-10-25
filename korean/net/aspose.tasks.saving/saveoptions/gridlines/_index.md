---
title: "SaveOptions.Gridlines"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 프로젝트 뷰에 표시되는 Gridline 목록을 가져오거나 설정합니다"
type: docs
weight: 60
url: /ko/net/aspose.tasks.saving/saveoptions/gridlines/
---
## SaveOptions.Gridlines property

프로젝트 뷰에 표시되는 [`Gridline`](../../../aspose.tasks.visualization/gridline/) 목록을 가져오거나 설정합니다.

```csharp
public List<Gridline> Gridlines { get; set; }
```

## 예제

레이아웃을 별도의 파일로 저장하는 방법을 보여줍니다.

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

// 프로젝트 레이아웃을 별도의 파일로 저장합니다.
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### 또 보기

* class [Gridline](../../../aspose.tasks.visualization/gridline/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


