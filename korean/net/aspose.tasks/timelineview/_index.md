---
title: "클래스 TimelineView"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TimelineView 클래스. 프로젝트의 타임라인 보기를 나타냅니다."
type: docs
weight: 2580
url: /ko/net/aspose.tasks/timelineview/
---
## TimelineView class

프로젝트의 타임라인 뷰를 나타냅니다.

```csharp
public class TimelineView : View
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [TimelineView](timelineview/)() | `TimelineView` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [DateFormat](../../aspose.tasks/timelineview/dateformat/) { get; set; } | 타임라인 보기에서 날짜를 형식화하는 방법을 나타내는 값을 가져오거나 설정합니다. |
| [DisplayOverlapped](../../aspose.tasks/timelineview/displayoverlapped/) { get; set; } | 여러 행에 겹쳐진 작업을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | 단일 보기에서 사용되는 필터를 가져오거나 설정합니다. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | 단일 보기의 그룹을 가져오거나 설정합니다. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Microsoft Project가 단일 보기의 필터를 강조 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | View 객체의 이름을 가져오거나 설정합니다. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | [`PageInfo`](../view/pageinfo/) 클래스의 인스턴스를 가져옵니다. mpp 파일 형식에 존재하는 페이지 설정 데이터를 나타냅니다. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | View 객체의 상위 항목을 가져옵니다. 읽기 전용 [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | 단일 보기의 화면 유형을 가져옵니다. 읽기 전용 [`ViewScreen`](../viewscreen/). |
| [ShowDates](../../aspose.tasks/timelineview/showdates/) { get; } | 날짜를 표시할지 여부를 나타내는 값을 가져옵니다. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Microsoft Project가 리본의 보기 또는 기타 보기 드롭다운 목록에 단일 보기 이름을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ShowPanZoom](../../aspose.tasks/timelineview/showpanzoom/) { get; set; } | 패닝 및 줌 컨트롤을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ShowTimescale](../../aspose.tasks/timelineview/showtimescale/) { get; set; } | 시간 눈금을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ShowToday](../../aspose.tasks/timelineview/showtoday/) { get; set; } | 오늘을 나타내는 선을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | 단일 보기의 테이블을 가져오거나 설정합니다. |
| [TextLinesCount](../../aspose.tasks/timelineview/textlinescount/) { get; set; } | 타임라인에서 작업을 표시하는 데 사용되는 라인 수를 나타내는 값을 가져오거나 설정합니다. |
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

&lt;see cref=\"Aspose.Tasks.TimelineView\" /&gt;와 작업하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 타임라인 보기를 초기화합니다.
var view = new TimelineView();

// 타임라인 보기에서 날짜를 형식화하는 방법을 나타내는 값을 설정합니다.
view.DateFormat = DateFormat.DateDddDd;
// 여러 행에 겹쳐진 작업을 표시할지 여부를 나타내는 값을 설정합니다.
view.DisplayOverlapped = true;
// 패닝 및 줌 컨트롤을 표시할지 여부를 나타내는 값을 설정합니다.
view.ShowPanZoom = true;
// 시간 눈금을 표시할지 여부를 나타내는 값을 설정합니다.
view.ShowTimescale = true;
// 오늘을 나타내는 선을 표시할지 여부를 나타내는 값을 설정합니다.
view.ShowToday = true;
// 타임라인에서 작업을 표시하는 데 사용되는 라인 수를 나타내는 값을 설정합니다.
view.TextLinesCount = 2;

// 여러 행에 겹쳐진 작업을 표시할지 여부를 나타내는 값을 가져옵니다.
Console.WriteLine("Show Dates: " + view.ShowDates);

// 보기를 프로젝트에 추가합니다.
project.Views.Add(view);

// 프로젝트에 테스트 데이터를 추가합니다.
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

project.Save(OutDir + "SetTimeScaleCount_out.pdf", SaveFileFormat.Pdf);
```

### 또 보기

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


