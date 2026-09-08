---
title: "SaveOptions.RollUpGanttBars"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 하위 작업이 요약 작업 막대에 표시될지 여부를 나타내는 값을 가져오거나 설정합니다. 하위 작업의 경우 Rollup 필드는 하위 작업 Gantt 막대에 대한 정보가 요약 작업 막대로 롤업되는지를 나타냅니다. 요약 작업의 경우 Rollup 필드는 요약 작업 막대가 롤업된 막대를 표시하는지를 나타냅니다. 하위 작업이 요약 작업에 롤업되려면 요약 작업에 대한 Rollup 필드를 Yes 로 설정해야 합니다."
type: docs
weight: 160
url: /ko/net/aspose.tasks.saving/saveoptions/rollupganttbars/
---
## SaveOptions.RollUpGanttBars property

요약 작업 막대에 하위 작업을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. 하위 작업의 경우, Rollup 필드는 하위 작업 Gantt 막대의 정보가 요약 작업 막대로 집계될지 여부를 나타냅니다. 요약 작업의 경우, Rollup 필드는 요약 작업 막대가 집계된 막대를 표시할지 여부를 나타냅니다. 하위 작업을 집계하려면 요약 작업에 대한 Rollup 필드를 Yes로 설정해야 합니다.

```csharp
public bool RollUpGanttBars { get; set; }
```

## 비고

Gantt 차트 뷰가 렌더링될 때만 적용됩니다.

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


