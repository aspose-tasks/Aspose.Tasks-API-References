---
title: "클래스 SaveOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.SaveOptions 클래스. 특정 형식으로 프로젝트를 저장할 때 사용자가 추가 옵션을 지정할 수 있도록 하는 클래스들의 추상 기본 클래스입니다."
type: docs
weight: 2190
url: /ko/net/aspose.tasks.saving/saveoptions/
---
## SaveOptions class

이것은 사용자가 특정 형식으로 프로젝트를 저장할 때 추가 옵션을 지정할 수 있도록 하는 클래스들을 위한 추상 기본 클래스입니다.

```csharp
public abstract class SaveOptions : SimpleSaveOptions
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | 프로젝트 보기에서 표시되는 [`BarStyle`](../../aspose.tasks.visualization/barstyle/) 클래스 인스턴스 목록을 가져오거나 설정합니다. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | 맞춤 페이지 크기를 포인트 단위로 가져오거나 설정합니다 (1 포인트 = 1/72 인치). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | 비작업 시간을 그릴지 여부를 나타내는 값을 가져오거나 설정합니다 (기본값은 TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | 렌더링을 종료할 날짜를 가져오거나 설정합니다. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | 행 높이를 내용에 맞게 늘릴지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | 프로젝트 뷰에 표시되는 [`Gridline`](../../aspose.tasks.visualization/gridline/) 목록을 가져오거나 설정합니다. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | 페이지 방향이 세로인지 여부를 나타내는 값을 가져오거나 설정합니다; 페이지 방향이 가로이면 false를 반환합니다. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | 범례를 렌더링하는 방법을 정의하는 값을 가져오거나 설정합니다. 기본값은 LegendDrawingOptions.OnEveryPage입니다. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | 페이지 범례에 렌더링될 막대를 정의하는 PageLegendItem 배열을 가져오거나 설정합니다. null인 경우 기본 항목이 렌더링됩니다. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | 중요 작업을 빨간색으로 표시할지 여부를 나타내는 값을 가져오거나 설정합니다 (기본값은 FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | 비작업 시간 색상을 가져오거나 설정합니다. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | 프로젝트 페이지 수를 가져오거나 설정합니다. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | 렌더링될 페이지 크기를 가져오거나 설정합니다 (기본값은 PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | 문서를 저장할 [`PresentationFormat`](./presentationformat/)을 가져오거나 설정합니다. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | 프로젝트가 그래픽 형식으로 저장될 때 단일 페이지로 렌더링할지 여부를 나타내는 값을 가져오거나 설정합니다. 렌더링된 프로젝트가 한 페이지에 맞도록 페이지 크기가 조정됩니다. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | 요약 작업 막대에 하위 작업을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. 하위 작업의 경우, Rollup 필드는 하위 작업 Gantt 막대의 정보가 요약 작업 막대로 집계될지 여부를 나타냅니다. 요약 작업의 경우, Rollup 필드는 요약 작업 막대가 집계된 막대를 표시할지 여부를 나타냅니다. 하위 작업을 집계하려면 요약 작업에 대한 Rollup 필드를 Yes로 설정해야 합니다. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 이 저장 옵션 개체가 사용될 경우 문서가 저장되는 형식을 가져오거나 설정합니다. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | 렌더링을 시작할 날짜를 가져오거나 설정합니다. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | 작업 링크 렌더링의 일부 측면을 사용자 지정하는 데 사용할 수 있는 콜백을 가져오거나 설정합니다. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 간트 차트 및 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 가져오거나 설정합니다. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 간트, 작업 시트 및 작업 사용 차트에 렌더링된 작업을 필터링하는 데 사용되는 조건을 가져오거나 설정합니다. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | 프로젝트 뷰 렌더링 중에 적용되는 텍스트 스타일 목록을 가져오거나 설정합니다. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | 프로젝트를 그래픽 형식으로 저장할 때 타임스케일(있는 경우)이 어떻게 렌더링되는지를 제어하는 데 사용되는 [`Timescale`](./timescale/) 값을 가져오거나 설정합니다. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | 타임스케일의 오른쪽 끝을 페이지 끝에 맞추는 방식을 정의하는 동작을 가져오거나 설정합니다. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Gantt 차트를 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | 렌더링할 보기 열 목록을 가져오거나 설정합니다 ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). 설정하지 않으면 작업 ID, 작업 이름, 시작 및 종료만 렌더링됩니다. View와 [`ViewSettings`](./viewsettings/) 속성이 모두 설정된 경우 View의 열이 ViewSettings의 열을 우선합니다. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | 렌더링할 보기 ([`View`](./view/))를 가져오거나 설정합니다. 이 옵션을 사용하여 PDF, HTML 또는 이미지 형식으로 저장할 보기를 명시적으로 지정할 수 있습니다. 이 속성이 설정되면 프로젝트 저장 시 [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) 속성이 무시됩니다. 보기는 다음 화면 중 하나여야 합니다 (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## 비고

SaveOptions 클래스에서 파생된 모든 클래스의 인스턴스는 문서를 저장할 때 사용자가 사용자 지정 옵션을 정의할 수 있도록 스트림 Save 또는 문자열 Save 오버로드에 전달됩니다.

## 예제

행 높이를 내용에 맞게 늘릴지 여부 옵션을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // 옵션 fit content를 true로 설정합니다
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### 또 보기

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


