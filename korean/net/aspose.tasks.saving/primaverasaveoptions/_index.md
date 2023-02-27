---
title: PrimaveraSaveOptions
second_title: .NET API 참조용 Aspose.Tasks
description: 프로젝트를 Primavera XER 형식으로 저장할 때 추가 옵션을 지정할 수 있습니다.
type: docs
weight: 1880
url: /ko/net/aspose.tasks.saving/primaverasaveoptions/
---
## PrimaveraSaveOptions class

프로젝트를 Primavera XER 형식으로 저장할 때 추가 옵션을 지정할 수 있습니다.

```csharp
public class PrimaveraSaveOptions : SaveOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PrimaveraSaveOptions](primaverasaveoptions/)() | 의 새 인스턴스를 초기화합니다.`PrimaveraSaveOptions` 클래스. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [ActivityIdIncrement](../../aspose.tasks.saving/primaverasaveoptions/activityidincrement/) { get; set; } | 활동 ID의 번호를 다시 지정하는 데 사용되는 증분을 가져오거나 설정합니다. |
| [ActivityIdPrefix](../../aspose.tasks.saving/primaverasaveoptions/activityidprefix/) { get; set; } | 활동 ID의 번호를 다시 지정하는 데 사용되는 접두사를 가져오거나 설정합니다. |
| [ActivityIdSuffix](../../aspose.tasks.saving/primaverasaveoptions/activityidsuffix/) { get; set; } | 활동 ID의 번호를 다시 지정하는 데 사용되는 접미사를 가져오거나 설정합니다. |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | 인스턴스 목록을 가져오거나 설정합니다.[`BarStyle`](../../aspose.tasks.visualization/barstyle/) 프로젝트 보기에 나타나는 클래스. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | 사용자 지정 페이지 크기를 포인트 단위로 가져오거나 설정합니다(1포인트 = 인치의 1/72). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | 휴무 시간을 그려야 하는지 여부를 나타내는 값을 가져오거나 설정합니다(기본값은 TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | 렌더링을 완료할 날짜를 가져오거나 설정합니다. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | 콘텐츠에 맞게 행 높이를 늘려야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | 보기의 달력 섹션이 마지막 페이지의 끝(오른쪽)에 렌더링되어야 하는지 여부를 가져오거나 설정합니다. 값이 false이면 페이지에 빈 공간이 있더라도 달력 섹션이 정확히 EndDate로 렌더링됩니다. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | 목록을 가져오거나 설정합니다.[`Gridline`](../../aspose.tasks.visualization/gridline/) 프로젝트 보기에 표시됩니다. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | 각 페이지에 범례를 표시할지 여부를 나타내는 값을 가져오거나 설정합니다(기본값은 TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | 중요한 작업을 빨간색으로 표시할지 여부를 나타내는 값을 가져오거나 설정합니다(기본값은 FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | 휴무 시간 색상을 가져오거나 설정합니다. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | 프로젝트의 페이지 수를 가져오거나 설정합니다. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | 렌더링할 페이지의 크기를 가져오거나 설정합니다(기본값은 PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | 가져오거나 설정합니다.[`PresentationFormat`](../saveoptions/presentationformat/) 문서가 저장될 위치. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | 프로젝트를 그래픽 형식으로 저장할 때 프로젝트를 단일 페이지로 렌더링할지 여부를 나타내는 값을 가져오거나 설정합니다. 렌더링된 프로젝트가 한 페이지에 맞도록 페이지 크기가 변경됩니다. |
| [RenumberActivityIds](../../aspose.tasks.saving/primaverasaveoptions/renumberactivityids/) { get; set; } | 활동 ID의 번호를 다시 지정해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | 요약 작업 표시줄의 하위 작업을 표시해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. 하위 작업의 경우 롤업 필드는 하위 작업 Gantt 막대의 정보가 요약 작업 표시줄에 롤업되는지 여부를 나타냅니다. 요약 작업의 경우 롤업 필드는 요약 작업 표시줄에 롤업된 막대가 표시되는지 여부를 나타냅니다. 요약 작업에 대한 롤업 필드가 예로 설정되어 있어야 하위 작업이 롤업됩니다. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | 이 저장 옵션 개체가 사용되는 경우 문서가 저장되는 형식을 가져오거나 설정합니다. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | 렌더링을 시작할 날짜를 가져오거나 설정합니다. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | Gantt 차트 및 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 가져오거나 설정합니다. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | Gantt, 작업 시트 및 작업 사용량 차트에서 렌더링된 작업을 필터링하는 데 사용되는 조건을 가져오거나 설정합니다. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | 인스턴스 목록을 가져오거나 설정합니다.[`TextStyle`](../../aspose.tasks.visualization/textstyle/) 프로젝트 보기에 나타나는 클래스. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | 가져오거나 설정합니다.[`Timescale`](../saveoptions/timescale/) 프로젝트를 그래픽 형식으로 저장할 때 시간 척도(있는 경우)를 렌더링하는 방법을 제어하는 데 사용되는 값입니다. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Gantt 차트를 렌더링할 때 그라데이션 브러시를 사용해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | 렌더링할 보기 열 목록을 가져오거나 설정합니다([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) ). 설정하지 않으면 작업 ID, 작업 이름, 시작 및 완료만 렌더링됩니다. 보기 및[`ViewSettings`](../saveoptions/viewsettings/)속성이 설정되면 View의 열이 ViewSettings. 의 열을 재정의합니다. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | 보기를 가져오거나 설정합니다([`View`](../saveoptions/view/) ) 렌더링합니다. 이 옵션을 사용하여 PDF, HTML 또는 이미지 형식으로 저장할 보기를 명시적으로 지정할 수 있습니다. 이 속성이 설정되면[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) 프로젝트 저장 시 속성은 무시됩니다. 보기는 다음 화면 중 하나여야 합니다(([`Screen`](../../aspose.tasks/view/screen/) )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### 또한보십시오

* class [SaveOptions](../saveoptions/)
* 네임스페이스 [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* 집회 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
