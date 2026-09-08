---
title: "SaveOptions.Timescale"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 프로젝트를 그래픽 형식으로 저장할 때 타임스케일이 존재하면 어떻게 렌더링되는지를 제어하는 Timescale 값을 가져오거나 설정합니다."
type: docs
weight: 200
url: /ko/net/aspose.tasks.saving/saveoptions/timescale/
---
## SaveOptions.Timescale property

`Timescale` 값을 가져오거나 설정합니다. 이 값은 프로젝트를 그래픽 형식으로 저장할 때 타임스케일이 존재하면 어떻게 렌더링되는지를 제어합니다.

```csharp
public Timescale Timescale { get; set; }
```

## 예제

렌더링할 최소 시간 기간을 설정하는 방법을 보여줍니다. 기본값은 <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.Timescale\">Days</see>입니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 한 페이지 이미지로 저장 (기본값은 Timescale.days).
project.Save(OutDir + "NewProductDevDays_out.jpeg", new ImageSaveOptions(SaveFileFormat.Jpeg));

// 한 페이지 이미지로 저장 (Timescale.ThirdsOfMonths).
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "NewProductDevThirdsOfMonths_out.jpeg", options);

// 한 페이지 이미지로 저장 (Timescale.Months).
options.Timescale = Timescale.Months;
project.Save(OutDir + "NewProductDevMonths_out.jpeg", options);
```

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

뷰 설정에 정의된 시간축 설정으로 작업 사용 보기를 렌더링하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// SaveOptions를 정의하고 TaskUsageView 시간축 설정을 사용하도록 지정합니다.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
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

### 또 보기

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


