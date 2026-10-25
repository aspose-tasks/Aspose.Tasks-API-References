---
title: "UsageView.MiddleTimescaleTier"
second_title: "Aspose.Tasks for .NET API 참조"
description: "UsageView 속성. 보기의 중간 시간축 계층 설정을 가져오거나 설정합니다. TimescaleTier"
type: docs
weight: 50
url: /ko/net/aspose.tasks/usageview/middletimescaletier/
---
## UsageView.MiddleTimescaleTier property

보기의 중간 시간축 계층 설정을 가져오거나 설정합니다. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier MiddleTimescaleTier { get; set; }
```

## 예제

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

### 또 보기

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


