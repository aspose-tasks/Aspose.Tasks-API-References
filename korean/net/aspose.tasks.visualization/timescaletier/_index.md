---
title: "Aspose.Tasks.Visualization.TimescaleTier 클래스. 간트 차트의 시간 눈금에 대한 단일 티어를 나타냅니다."
second_title: "Aspose.Tasks for .NET API 참조"
description: "`TimescaleTier` 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 3450
url: /ko/net/aspose.tasks.visualization/timescaletier/
---
## TimescaleTier class

Gantt 차트의 시간축 단일 계층을 나타냅니다.

```csharp
public sealed class TimescaleTier
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [TimescaleTier](timescaletier/#constructor)() | 티어의 각 시간 기간 내에서 레이블을 정렬하는 방법을 가져오거나 설정합니다 ([`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TimescaleTier](timescaletier/#constructor_1)(TimescaleUnit, int) | 티어의 각 시간 기간 내에서 레이블을 정렬하는 방법을 가져오거나 설정합니다 ([`HorizontalStringAlignment`](../horizontalstringalignment/)). |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Alignment](../../aspose.tasks.visualization/timescaletier/alignment/) { get; set; } | 티어에 레이블을 표시할 시간 단위 간격을 가져오거나 설정합니다. 기본값은 1입니다. |
| [Count](../../aspose.tasks.visualization/timescaletier/count/) { get; set; } | 이 티어에서 날짜 눈금 렌더링을 처리하기 위한 콜백 함수를 가져오거나 설정합니다. |
| [DateTimeConverter](../../aspose.tasks.visualization/timescaletier/datetimeconverter/) { get; set; } | 시간 눈금 티어의 날짜 레이블 [`DateLabel`](../datelabel/)을 가져오거나 설정합니다. |
| [Label](../../aspose.tasks.visualization/timescaletier/label/) { get; set; } | 시간 기간이 여러 페이지에 걸칠 때 각 페이지에 날짜 레이블을 렌더링할지 여부를 정의하는 플래그를 가져오거나 설정합니다. 값이 'true'이면, 기간이 여러 페이지에 걸칠 때 해당 기간의 날짜 레이블이 각 페이지에 렌더링됩니다. 값이 'false'이면, [`Alignment`](./alignment/) 속성 값에 따라 날짜 레이블이 한 번만 렌더링됩니다. |
| [RenderLabelOnEachPage](../../aspose.tasks.visualization/timescaletier/renderlabeloneachpage/) { get; set; } | 티어에서 시간 기간을 구분하는 눈금 표시를 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ShowTicks](../../aspose.tasks.visualization/timescaletier/showticks/) { get; set; } | 시간 눈금 티어의 시간 눈금 단위 [`TimescaleUnit`](../timescaleunit/)를 가져오거나 설정합니다. 기본값은 [`Days`](../timescaleunit/)입니다. |
| [Unit](../../aspose.tasks.visualization/timescaletier/unit/) { get; set; } | 티어 레이블을 회계 연도에 기반할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [UsesFiscalYear](../../aspose.tasks.visualization/timescaletier/usesfiscalyear/) { get; set; } | 시간 눈금 티어 레이블을 사용자 정의하는 방법을 보여줍니다. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


