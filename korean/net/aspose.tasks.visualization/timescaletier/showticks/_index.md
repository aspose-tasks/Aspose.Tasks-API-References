---
title: "TimescaleTier.ShowTicks"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TimescaleTier 속성. 티어에서 시간 기간을 구분하는 눈금 표시를 할지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 70
url: /ko/net/aspose.tasks.visualization/timescaletier/showticks/
---
## TimescaleTier.ShowTicks property

시간 눈금 티어의 시간 눈금 단위 [`TimescaleUnit`](../timescaleunit/)를 가져오거나 설정합니다. 기본값은 [`Days`](../timescaleunit/)입니다.

```csharp
public bool ShowTicks { get; set; }
```

## 예제

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

* class [TimescaleTier](../)
* namespace [Aspose.Tasks.Visualization](../../timescaletier/)
* assembly [Aspose.Tasks](../../../)


