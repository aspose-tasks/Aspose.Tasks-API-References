---
title: "Aspose::Tasks::Saving::SaveOptions 클래스"
linktitle: "SaveOptions"
articleTitle: "SaveOptions"
second_title: "C++용 Aspose.Tasks"
description: "이는 사용자가 프로젝트를 특정 형식으로 저장할 때 추가 옵션을 지정할 수 있도록 허용하는 클래스들의 추상 기본 클래스입니다."
type: docs
weight: 10
url: /ko/cpp/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

**Inherits:** Aspose::Tasks::Saving::SimpleSaveOptions

이는 사용자가 프로젝트를 특정 형식으로 저장할 때 추가 옵션을 지정할 수 있도록 허용하는 클래스들의 추상 기본 클래스입니다.

SaveOptions 클래스에서 파생된 모든 클래스의 인스턴스는 문서를 저장할 때 사용자가 사용자 정의 옵션을 정의할 수 있도록 스트림 Save 또는 문자열 Save 오버로드에 전달됩니다.

## 메서드

| 이름 | 설명 |
| --- | --- |
| [get_BarStyles](./get_barstyles/) | 프로젝트 뷰에 나타나는 BarStyle 클래스 인스턴스 목록을 가져옵니다. |
| [get_CustomPageSize](./get_custompagesize/) | 포인트 단위(1포인트 = 1/72인치)의 사용자 지정 페이지 크기를 가져옵니다. |
| [get_DrawNonWorkingTime](./get_drawnonworkingtime/) | 비작업 시간이 그려져야 하는지를 나타내는 값을 가져옵니다(기본값은 TRUE). |
| [get_EndDate](./get_enddate/) | 렌더링을 종료할 날짜를 가져옵니다. |
| [get_FitContent](./get_fitcontent/) | 행 높이를 내용에 맞게 늘려야 하는지를 나타내는 값을 가져옵니다. |
| [get_FitTimescaleToEndOfPage](./get_fittimescaletoendofpage/) | 뷰의 캘린더 섹션을 마지막 페이지의 끝(오른쪽)까지 렌더링할지 여부를 가져옵니다. 값이 false인 경우 페이지에 빈 공간이 있더라도 캘린더 섹션은 EndDate까지 정확히 렌더링됩니다. |
| [get_Gridlines](./get_gridlines/) | 프로젝트 뷰에 나타나는 Gridline 목록을 가져옵니다. |
| [get_IsPortrait](./get_isportrait/) | 페이지 방향이 세로인지 여부를 나타내는 값을 가져옵니다; 페이지 방향이 가로인 경우 false를 반환합니다. |
| [get_LegendDrawingOptions](./get_legenddrawingoptions/) | 범례를 렌더링하는 방법을 정의하는 값을 가져옵니다. 기본값은 LegendDrawingOptions.OnEveryPage입니다. |
| [get_LegendItems](./get_legenditems/) | 페이지 범례에 렌더링될 막대를 정의하는 PageLegendItem 배열을 가져옵니다. null인 경우 기본 항목이 렌더링됩니다. |
| [get_MarkCriticalTasks](./get_markcriticaltasks/) | 중요 작업을 빨간색으로 표시할지 여부를 나타내는 값을 가져옵니다(기본값은 FALSE). |
| [get_NonWorkingTimeColor](./get_nonworkingtimecolor/) | 비작업 시간 색상을 가져옵니다. |
| [get_PageCount](./get_pagecount/) | 프로젝트의 페이지 수를 가져옵니다. |
| [get_PageSize](./get_pagesize/) | 렌더링될 페이지 크기를 가져옵니다(기본값은 PageSize.A4). |
| [get_PresentationFormat](./get_presentationformat/) | 문서가 저장될 PresentationFormat을 가져옵니다. |
| [get_RenderToSinglePage](./get_rendertosinglepage/) | 프로젝트가 그래픽 형식으로 저장될 때 단일 페이지로 렌더링될지 여부를 나타내는 값을 가져옵니다. 페이지 크기가 조정되어 렌더링된 프로젝트가 한 페이지에 맞게 됩니다. |
| [get_RollUpGanttBars](./get_rollupganttbars/) | 요약 작업 막대에 하위 작업이 표시될지 여부를 나타내는 값을 가져옵니다. 하위 작업의 경우 Rollup 필드는 하위 작업 Gantt 막대의 정보가 요약 작업 막대로 롤업되는지를 나타냅니다. 요약 작업의 경우 Rollup 필드는 요약 작업 막대가 롤업된 막대를 표시하는지를 나타냅니다. 하위 작업이 롤업되려면 요약 작업의 Rollup 필드를 Yes로 설정해야 합니다. |
| [get_StartDate](./get_startdate/) | 렌더링을 시작할 날짜를 가져옵니다. |
| [get_TextStyles](./get_textstyles/) | 프로젝트 뷰 렌더링 중 적용되는 텍스트 스타일 목록을 가져옵니다. |
| [get_Timescale](./get_timescale/) | 프로젝트를 그래픽 형식으로 저장할 때 타임스케일(존재하는 경우)이 어떻게 렌더링되는지를 제어하는 Timescale 값을 가져옵니다. |
| [get_TimescaleFitBehavior](./get_timescalefitbehavior/) | 타임스케일의 오른쪽 끝을 페이지 끝에 맞추는 방식을 정의하는 동작을 가져옵니다. |
| [get_UseGradientBrush](./get_usegradientbrush/) | Gantt 차트를 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 가져옵니다. |
| [get_View](./get_view/) | 렌더링할 보기 열 목록을 가져옵니다 ( GanttChartColumn ). 설정되지 않은 경우 작업 ID, 작업 이름, 시작 및 종료만 렌더링됩니다. View와 ViewSettings 속성이 모두 설정된 경우, View의 열이 ViewSettings의 열을 우선합니다. |
| [get_ViewSettings](./get_viewsettings/) | 렌더링할 보기 ( View )를 가져옵니다. 이 옵션을 사용하여 PDF, HTML 또는 이미지 형식으로 저장할 보기를 명시적으로 지정할 수 있습니다. 이 속성이 설정되면 프로젝트를 저장할 때 Visualization::PresentationFormat 속성이 무시됩니다. View는 다음 화면 중 하나여야 합니다 (( Aspose::Tasks::View::Screen )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |
| [set_BarStyles](./set_barstyles/) | 프로젝트 보기에서 표시되는 BarStyle 클래스 인스턴스 목록을 설정합니다. |
| [set_CustomPageSize](./set_custompagesize/) | 포인트 단위(1포인트 = 1/72인치)로 사용자 정의 페이지 크기를 설정합니다. |
| [set_DrawNonWorkingTime](./set_drawnonworkingtime/) | 비작업 시간을 그릴지 여부를 나타내는 값을 설정합니다(기본값은 TRUE). |
| [set_EndDate](./set_enddate/) | 렌더링을 종료할 날짜를 설정합니다. |
| [set_FitContent](./set_fitcontent/) | 행 높이를 내용에 맞게 늘릴지 여부를 나타내는 값을 설정합니다. |
| [set_FitTimescaleToEndOfPage](./set_fittimescaletoendofpage/) | 보기에 대한 캘린더 섹션을 마지막 페이지의 끝(오른쪽)까지 렌더링할지 여부를 설정합니다. 값이 false인 경우 페이지에 빈 공간이 있더라도 캘린더 섹션은 EndDate까지 정확히 렌더링됩니다. |
| [set_Gridlines](./set_gridlines/) | 프로젝트 보기에서 표시되는 Gridline 목록을 설정합니다. |
| [set_IsPortrait](./set_isportrait/) | 페이지 방향이 세로인지 여부를 나타내는 값을 설정합니다; 페이지 방향이 가로인 경우 false를 반환합니다. |
| [set_LegendDrawingOptions](./set_legenddrawingoptions/) | 범례를 렌더링하는 방법을 정의하는 값을 설정합니다. 기본값은 LegendDrawingOptions.OnEveryPage입니다. |
| [set_LegendItems](./set_legenditems/) | 페이지 범례에 렌더링할 막대를 정의하는 PageLegendItem 배열을 설정합니다. null인 경우 기본 항목이 렌더링됩니다. |
| [set_MarkCriticalTasks](./set_markcriticaltasks/) | 중요 작업을 빨간색으로 표시할지 여부를 나타내는 값을 설정합니다(기본값은 FALSE). |
| [set_NonWorkingTimeColor](./set_nonworkingtimecolor/) | 비작업 시간 색상을 설정합니다. |
| [set_PageSize](./set_pagesize/) | 렌더링할 페이지 크기를 설정합니다(기본값은 PageSize.A4). |
| [set_PresentationFormat](./set_presentationformat/) | 문서가 저장될 PresentationFormat을 설정합니다. |
| [set_RenderToSinglePage](./set_rendertosinglepage/) | 프로젝트를 그래픽 형식으로 저장할 때 단일 페이지에 렌더링할지 여부를 나타내는 값을 설정합니다. 렌더링된 프로젝트가 한 페이지에 맞도록 페이지 크기가 조정됩니다. |
| [set_RollUpGanttBars](./set_rollupganttbars/) | 요약 작업 막대에 하위 작업을 표시할지 여부를 나타내는 값을 설정합니다. 하위 작업의 경우 Rollup 필드는 하위 작업 Gantt 막대의 정보가 요약 작업 막대로 롤업될지 여부를 나타냅니다. 요약 작업의 경우 Rollup 필드는 요약 작업 막대가 롤업된 막대를 표시할지 여부를 나타냅니다. 하위 작업이 롤업되려면 요약 작업에 대한 Rollup 필드를 Yes로 설정해야 합니다. |
| [set_StartDate](./set_startdate/) | 렌더링을 시작할 날짜를 설정합니다. |
| [set_TextStyles](./set_textstyles/) | 프로젝트 보기 렌더링 중에 적용되는 텍스트 스타일 목록을 설정합니다. |
| [set_Timescale](./set_timescale/) | 프로젝트를 그래픽 형식으로 저장할 때 타임스케일(있는 경우)의 렌더링 방식을 제어하는 Timescale 값을 설정합니다. |
| [set_TimescaleFitBehavior](./set_timescalefitbehavior/) | 타임스케일의 오른쪽 끝을 페이지 끝에 맞추는 방식을 정의하는 동작을 설정합니다. |
| [set_UseGradientBrush](./set_usegradientbrush/) | Gantt 차트를 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 설정합니다. |
| [set_View](./set_view/) | 렌더링할 보기 열 목록을 설정합니다 ( GanttChartColumn ). 설정되지 않으면 작업 ID, 작업 이름, 시작 및 종료만 렌더링됩니다. View와 ViewSettings 속성이 모두 설정된 경우, View의 열이 ViewSettings의 열을 우선합니다. |
| [set_ViewSettings](./set_viewsettings/) | 렌더링할 보기 ( View )를 설정합니다. 이 옵션을 사용하여 PDF, HTML 또는 이미지 형식으로 저장할 보기를 명시적으로 지정할 수 있습니다. 이 속성이 설정되면 프로젝트를 저장할 때 Visualization::PresentationFormat 속성이 무시됩니다. View는 다음 화면 중 하나여야 합니다 (( Aspose::Tasks::View::Screen )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

