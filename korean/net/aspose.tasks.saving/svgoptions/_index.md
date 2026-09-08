---
title: "SvgOptions 클래스"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.SvgOptions 클래스. 프로젝트 페이지를 SVG로 렌더링할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 2230
url: /ko/net/aspose.tasks.saving/svgoptions/
---
## SvgOptions class

프로젝트 페이지를 SVG로 렌더링할 때 추가 옵션을 지정할 수 있습니다.

```csharp
public class SvgOptions : SaveOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [SvgOptions](svgoptions/)() | `SvgOptions` 클래스의 새 인스턴스를 초기화하며, 이를 사용하여 프로젝트를 SVG 형식으로 저장할 수 있습니다. |

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
| [PageSavingCallback](../../aspose.tasks.saving/svgoptions/pagesavingcallback/) { get; set; } | 각 렌더링된 페이지에 대한 출력 스트림을 가져오는 데 사용되는 사용자 정의 구현 콜백을 가져오거나 설정합니다. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | 렌더링될 페이지 크기를 가져오거나 설정합니다 (기본값은 PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | 문서가 저장될 [`PresentationFormat`](../saveoptions/presentationformat/)을 가져오거나 설정합니다. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | 프로젝트가 그래픽 형식으로 저장될 때 단일 페이지로 렌더링할지 여부를 나타내는 값을 가져오거나 설정합니다. 렌더링된 프로젝트가 한 페이지에 맞도록 페이지 크기가 조정됩니다. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | 요약 작업 막대에 하위 작업을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. 하위 작업의 경우, Rollup 필드는 하위 작업 Gantt 막대의 정보가 요약 작업 막대로 집계될지 여부를 나타냅니다. 요약 작업의 경우, Rollup 필드는 요약 작업 막대가 집계된 막대를 표시할지 여부를 나타냅니다. 하위 작업을 집계하려면 요약 작업에 대한 Rollup 필드를 Yes로 설정해야 합니다. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 이 저장 옵션 개체가 사용될 경우 문서가 저장되는 형식을 가져오거나 설정합니다. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | 렌더링을 시작할 날짜를 가져오거나 설정합니다. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | 작업 링크 렌더링의 일부 측면을 사용자 지정하는 데 사용할 수 있는 콜백을 가져오거나 설정합니다. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 간트 차트 및 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 가져오거나 설정합니다. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 간트, 작업 시트 및 작업 사용 차트에 렌더링된 작업을 필터링하는 데 사용되는 조건을 가져오거나 설정합니다. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | 프로젝트 뷰 렌더링 중에 적용되는 텍스트 스타일 목록을 가져오거나 설정합니다. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | 프로젝트를 그래픽 형식으로 저장할 때 타임스케일(있는 경우)이 렌더링되는 방식을 제어하는 ​​[`Timescale`](../saveoptions/timescale/) 값을 가져오거나 설정합니다. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | 타임스케일의 오른쪽 끝을 페이지 끝에 맞추는 방식을 정의하는 동작을 가져오거나 설정합니다. |
| override [UseGradientBrush](../../aspose.tasks.saving/svgoptions/usegradientbrush/) { get; set; } | 프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 결정합니다. 현재 SVG로 렌더링할 때 그라디언트 브러시 사용은 지원되지 않습니다. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | 렌더링할 뷰 열 목록을 가져오거나 설정합니다 ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). 설정되지 않으면 작업 ID, 작업 이름, 시작 및 종료만 렌더링됩니다. View와 [`ViewSettings`](../saveoptions/viewsettings/) 속성이 모두 설정된 경우, View의 열이 ViewSettings의 열을 우선합니다. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | 렌더링할 뷰 ([`View`](../saveoptions/view/))를 가져오거나 설정합니다. 이 옵션을 사용하여 PDF, HTML 또는 이미지 형식으로 저장될 뷰를 명시적으로 지정할 수 있습니다. 이 속성이 설정되면 프로젝트 저장 시 [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) 속성이 무시됩니다. 뷰는 다음 화면 중 하나여야 합니다 (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## 예제

프로젝트를 SVG 파일로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // 문서가 저장될 <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" />을 설정합니다.
                            PresentationFormat = PresentationFormat.GanttChart,

                            // 행 높이를 내용에 맞게 늘릴지 여부를 나타내는 값을 설정합니다.
                            FitContent = true,

                            // 렌더링할 최소 시간 기간을 설정합니다. 기본값은 <see cref="P:Aspose.Tasks.Saving.SaveOptions.Timescale">Days</see>입니다.
                            Timescale = Timescale.ThirdsOfMonths,

                            // 프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 결정합니다.
                            // 현재 SVG로 렌더링할 때 그라디언트 브러시 사용은 지원되지 않습니다.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### 또 보기

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


