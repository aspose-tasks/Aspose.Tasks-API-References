---
title: "SaveOptions.MarkCriticalTasks"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 중요 작업을 빨간색으로 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. 기본값은 FALSE입니다."
type: docs
weight: 100
url: /ko/net/aspose.tasks.saving/saveoptions/markcriticaltasks/
---
## SaveOptions.MarkCriticalTasks property

중요 작업을 빨간색으로 표시할지 여부를 나타내는 값을 가져오거나 설정합니다 (기본값은 FALSE).

```csharp
public bool MarkCriticalTasks { get; set; }
```

## 예제

이미지 파일 형식으로 저장할 때 중요 작업을 인쇄하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png)
{
    StartDate = project.Get(Prj.StartDate).AddDays(-3),
    EndDate = project.Get(Prj.FinishDate),
    MarkCriticalTasks = true,
    LegendDrawingOptions = LegendDrawingOptions.NoLegend,
    Gridlines = new List<Gridline>()
};

var gridline = new Gridline { GridlineType = GridlineType.GanttRow, Color = Color.CornflowerBlue, Pattern = LinePattern.Dashed };
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles1_out.png", options);

// 프로젝트 레이아웃을 별도의 파일로 저장합니다.
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### 또 보기

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


