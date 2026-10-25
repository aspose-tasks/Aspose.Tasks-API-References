---
title: "클래스 GanttChartView"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.GanttChartView 클래스. GanttChart 뷰를 나타냅니다."
type: docs
weight: 710
url: /ko/net/aspose.tasks/ganttchartview/
---
## GanttChartView class

GanttChart 보기를 나타냅니다.

```csharp
public class GanttChartView : View
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [GanttChartView](ganttchartview/)() | `GanttChartView` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [AutoFilters](../../aspose.tasks/ganttchartview/autofilters/) { get; } | Gantt 차트 뷰의 자동 필터 목록을 가져옵니다. |
| [BarRounding](../../aspose.tasks/ganttchartview/barrounding/) { get; set; } | 막대가 가장 가까운 날짜로 반올림되는지 여부를 나타내는 값을 가져오거나 설정합니다. 기본값은 True입니다. |
| [BarSize](../../aspose.tasks/ganttchartview/barsize/) { get; set; } | Gantt 차트의 Gantt 막대 높이(포인트)를 가져오거나 설정합니다. |
| [BarStyles](../../aspose.tasks/ganttchartview/barstyles/) { get; } | Gantt 차트 뷰의 상위(공통) 막대 스타일 목록을 가져옵니다. [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle/). |
| [BottomTimescaleTier](../../aspose.tasks/ganttchartview/bottomtimescaletier/) { get; set; } | 뷰 하단 타임스케일 티어의 설정을 가져오거나 설정합니다. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [CustomBarStyles](../../aspose.tasks/ganttchartview/custombarstyles/) { get; } | Gantt 차트 뷰의 사용자 지정 작업별 막대 스타일 목록을 가져옵니다. [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle/). |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | 단일 보기에서 사용되는 필터를 가져오거나 설정합니다. |
| [Gridlines](../../aspose.tasks/ganttchartview/gridlines/) { get; set; } | Gantt 차트 뷰의 [`Gridlines`](./gridlines/) 목록을 가져오거나 설정합니다. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | 단일 보기의 그룹을 가져오거나 설정합니다. |
| [HideRollupBarsWhenSummaryExpanded](../../aspose.tasks/ganttchartview/hiderollupbarswhensummaryexpanded/) { get; set; } | 요약 작업을 확장할 때 롤업 막대가 숨겨지는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Microsoft Project가 단일 보기의 필터를 강조 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [MiddleTimescaleTier](../../aspose.tasks/ganttchartview/middletimescaletier/) { get; set; } | 보기의 중간 시간축 단계 설정을 가져오거나 설정합니다. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | View 객체의 이름을 가져오거나 설정합니다. |
| [NonWorkingTimeColor](../../aspose.tasks/ganttchartview/nonworkingtimecolor/) { get; set; } | 비작업 시간 색상을 가져오거나 설정합니다. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | [`PageInfo`](../view/pageinfo/) 클래스의 인스턴스를 가져옵니다. mpp 파일 형식에 존재하는 페이지 설정 데이터를 나타냅니다. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | View 객체의 상위 항목을 가져옵니다. 읽기 전용 [`Project`](../project/). |
| [ProgressLines](../../aspose.tasks/ganttchartview/progresslines/) { get; set; } | Gantt 차트 뷰의 진행 라인을 가져오거나 설정합니다. [`ProgressLines`](./progresslines/). |
| [RollUpGanttBars](../../aspose.tasks/ganttchartview/rollupganttbars/) { get; set; } | Gantt 차트의 막대를 롤업해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | 단일 보기의 화면 유형을 가져옵니다. 읽기 전용 [`ViewScreen`](../viewscreen/). |
| [ShowBarSplits](../../aspose.tasks/ganttchartview/showbarsplits/) { get; set; } | Gantt 차트의 작업 분할을 표시해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ShowDrawings](../../aspose.tasks/ganttchartview/showdrawings/) { get; set; } | Gantt 차트의 도면을 표시해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Microsoft Project가 리본의 보기 또는 기타 보기 드롭다운 목록에 단일 보기 이름을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | 단일 보기의 테이블을 가져오거나 설정합니다. |
| [TableTextStyles](../../aspose.tasks/ganttchartview/tabletextstyles/) { get; } | Gantt 차트 뷰의 테이블 텍스트 스타일 목록을 가져옵니다. [`TableTextStyle`](../../aspose.tasks.visualization/tabletextstyle/). |
| [TextStyles](../../aspose.tasks/ganttchartview/textstyles/) { get; set; } | Gantt 차트 뷰의 [`TextStyle`](../../aspose.tasks.visualization/textstyle/) 목록을 가져오거나 설정합니다. |
| [TimescaleSizePercentage](../../aspose.tasks/ganttchartview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/ganttchartview/toptimescaletier/) { get; set; } | 보기의 상단 시간축 단계 설정을 가져오거나 설정합니다. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Type](../../aspose.tasks/view/type/) { get; } | 단일 보기의 항목 유형(예: 작업 또는 리소스)을 가져옵니다. 읽기 전용 [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | 보기의 고유 식별자를 가져옵니다. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | 보기에서 [`OleObject`](../oleobject/)의 배치 및 모양을 나타내는 객체 컬렉션을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | 현재 인스턴스를 동일한 유형의 다른 객체와 비교하고, 현재 인스턴스가 정렬 순서에서 앞선, 뒤에 있거나 같은 위치에 있는지를 나타내는 정수를 반환합니다. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | [`Resource`](../resource/) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |

## 예제

시간 눈금 계층을 수정하는 방법을 보여줍니다.

```csharp
var project = new Project();

// Gantt 차트 뷰 초기화
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// 시간 눈금 개수를 설정합니다
view.TopTimescaleTier.Count = 2;
view.TopTimescaleTier.Unit = TimescaleUnit.Quarters;
view.TopTimescaleTier.Label = DateLabel.QuarterQQyy;
view.TopTimescaleTier.ShowTicks = false;

view.MiddleTimescaleTier.Count = 2;
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
view.MiddleTimescaleTier.ShowTicks = false;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayDdd;
view.BottomTimescaleTier.Count = 2;
view.BottomTimescaleTier.ShowTicks = false;

// 프로젝트에 Gantt 차트 뷰를 추가합니다
project.Views.Add(view);

// 프로젝트에 테스트 데이터를 추가합니다.
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// 설정한 시간 눈금 설정(view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier)을 사용하여 시간 눈금을 렌더링하려면 'Timescale.DefinedInView' 옵션을 사용합니다.
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

### 또 보기

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


