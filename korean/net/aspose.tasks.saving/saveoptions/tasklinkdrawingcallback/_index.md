---
title: "SaveOptions.TaskLinkDrawingCallback"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 작업 링크 렌더링의 일부 측면을 사용자 정의하는 데 사용할 수 있는 콜백을 가져오거나 설정합니다"
type: docs
weight: 180
url: /ko/net/aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/
---
## SaveOptions.TaskLinkDrawingCallback property

작업 링크 렌더링의 일부 측면을 사용자 지정하는 데 사용할 수 있는 콜백을 가져오거나 설정합니다.

```csharp
public TaskLinkDrawingCallbackDelegate TaskLinkDrawingCallback { get; set; }
```

## 비고

Gantt 차트 뷰가 렌더링될 때만 적용됩니다.

## 예제

간트 차트 뷰를 렌더링할 때 작업 링크의 색상을 사용자 지정하기 위해 TaskLinkDrawingCallback을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "schedule-conflict.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A3;
saveOptions.StartDate = project.StartDate.AddDays(-2);
saveOptions.EndDate = project.FinishDate.AddDays(2);
saveOptions.ViewSettings = view;
saveOptions.TaskLinkDrawingCallback += delegate(TaskLinkDrawingArgs args)
{
    if (args.Link.LinkType == TaskLinkType.FinishToFinish)
    {
        args.Color = Color.Red;
    }
};

project.Save(OutDir + "WorkWithTaskLinkDrawingCallback_out.pdf", saveOptions);
```

### 또 보기

* delegate [TaskLinkDrawingCallbackDelegate](../../tasklinkdrawingcallbackdelegate/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


