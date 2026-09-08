---
title: "SaveOptions.TimescaleFitBehavior"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 타임스케일의 오른쪽 끝을 페이지 끝에 맞추는 방법을 정의하는 동작을 가져오거나 설정합니다"
type: docs
weight: 210
url: /ko/net/aspose.tasks.saving/saveoptions/timescalefitbehavior/
---
## SaveOptions.TimescaleFitBehavior property

타임스케일의 오른쪽 끝을 페이지 끝에 맞추는 방식을 정의하는 동작을 가져오거나 설정합니다.

```csharp
public TimescaleFitBehavior TimescaleFitBehavior { get; set; }
```

## 예제

TimescaleFitBehavior를 사용하여 Gantt 차트의 시간축을 마지막 페이지 끝에 맞추는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### 또 보기

* enum [TimescaleFitBehavior](../../../aspose.tasks.visualization/timescalefitbehavior/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


