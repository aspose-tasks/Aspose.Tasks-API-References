---
title: "GanttChartView.MiddleTimescaleTier"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GanttChartView 속성. 보기의 중간 시간축 티어 설정을 가져오거나 설정합니다. TimescaleTier"
type: docs
weight: 100
url: /ko/net/aspose.tasks/ganttchartview/middletimescaletier/
---
## GanttChartView.MiddleTimescaleTier property

보기의 중간 시간축 계층 설정을 가져오거나 설정합니다. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier MiddleTimescaleTier { get; set; }
```

## 예제

저장 옵션을 통해 시간축 티어를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

GanttChartView ganttChartView = (GanttChartView) project.Views.ToList()[0];

// Gantt Chart 보기의 시간축 티어를 설정합니다
ganttChartView.MiddleTimescaleTier.Unit = TimescaleUnit.Months;
ganttChartView.MiddleTimescaleTier.Count = 1;
ganttChartView.MiddleTimescaleTier.Label = DateLabel.MonthMmmm;

ganttChartView.BottomTimescaleTier.Unit = TimescaleUnit.Days;
ganttChartView.BottomTimescaleTier.Count = 1;
ganttChartView.BottomTimescaleTier.Label = DateLabel.DayDddDd;

// ...
var options = new ImageSaveOptions(SaveFileFormat.Png)
{
    Timescale = Timescale.DefinedInView
};

// ...

// 프로젝트를 이미지로 저장합니다
project.Save(OutDir + "WorkWithTimescaleTier_out.png", options);
```

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

작업 링크 추가

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// 시간 눈금 티어 조정
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// 상위 티어 조정

// 간트 차트 보기의 최상위 시간 눈금 티어를 설정합니다.
// 시간 눈금 티어에 대한 시간 눈금 단위 <see cref="T:Aspose.Tasks.Visualization.TimescaleUnit" />를 설정합니다.
view.MiddleTimescaleTier = new TimescaleTier();
// 티어에 레이블을 표시할 시간 단위 간격을 설정합니다.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// 시간 눈금 티어에 대한 날짜 레이블 <see cref="T:Aspose.Tasks.Visualization.DateLabel" />을 설정합니다.
view.MiddleTimescaleTier.Count = 1;
// 티어의 각 시간 기간 내에서 레이블을 정렬하는 방법을 설정합니다 (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// 계층의 각 시간 기간 내에서 레이블을 정렬하는 방법을 설정합니다 (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// 계층에서 시간 기간을 구분하는 눈금 표시를 표시할지 여부를 나타내는 값을 설정합니다.
view.MiddleTimescaleTier.ShowTicks = true;
// 계층 레이블을 회계 연도에 기반하도록 할지 여부를 나타내는 값을 설정합니다.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// 시각화를 개선하기 위해 추가되었습니다.
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// 중간 계층 날짜를 사용자 지정합니다.
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// 뷰에 정의된 타임스케일 설정(view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier)을 사용하여 타임스케일을 렌더링하려면 'Timescale.DefinedInView' 옵션을 사용합니다.
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### 또 보기

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


