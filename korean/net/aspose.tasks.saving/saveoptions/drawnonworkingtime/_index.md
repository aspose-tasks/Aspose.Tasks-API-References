---
title: "SaveOptions.DrawNonWorkingTime"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 비작업 시간을 그릴지 여부를 나타내는 값을 가져오거나 설정합니다. 기본값은 TRUE입니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.saving/saveoptions/drawnonworkingtime/
---
## SaveOptions.DrawNonWorkingTime property

비작업 시간을 그릴지 여부를 나타내는 값을 가져오거나 설정합니다 (기본값은 TRUE).

```csharp
public bool DrawNonWorkingTime { get; set; }
```

## 예제

요약 작업 막대의 하위 작업을 집계해야 함을 나타내는 값을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // 또는
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### 또 보기

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


