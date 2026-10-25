---
title: "TimelineView.ShowDates"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TimelineView 속성. 날짜를 표시할지 여부를 나타내는 값을 가져옵니다"
type: docs
weight: 40
url: /ko/net/aspose.tasks/timelineview/showdates/
---
## TimelineView.ShowDates property

날짜를 표시할지 여부를 나타내는 값을 가져옵니다.

```csharp
public bool ShowDates { get; }
```

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

* class [TimelineView](../)
* namespace [Aspose.Tasks](../../timelineview/)
* assembly [Aspose.Tasks](../../../)


