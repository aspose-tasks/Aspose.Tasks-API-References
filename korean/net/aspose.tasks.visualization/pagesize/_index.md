---
title: "Enum PageSize"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.PageSize 열거형. 페이지 크기를 지정합니다."
type: docs
weight: 3250
url: /ko/net/aspose.tasks.visualization/pagesize/
---
## PageSize enumeration

페이지 크기를 지정합니다.

```csharp
public enum PageSize
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Letter | `0` | Letter 페이지의 크기(포인트)는 792 × 612입니다. |
| Ledger | `1` | Ledger 페이지의 크기(포인트)는 1224 × 792입니다. |
| A0 | `2` | A0 페이지의 크기(포인트)는 3371 × 2384입니다. |
| A1 | `3` | A1 페이지의 크기(포인트)는 2384 × 1685입니다. |
| A2 | `4` | A2 페이지의 크기(포인트)는 1684 × 1190입니다. |
| A3 | `5` | A3 페이지의 크기(포인트)는 1190 × 842입니다. |
| A4 | `6` | A4 페이지의 크기(포인트)는 842 × 595입니다. |
| DefinedInView | `7` | View의 [`PageSettings`](../pagesettings/)에 정의된 페이지 크기를 사용합니다 (View.PageInfo.PageSettings). |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


