---
title: "델리게이트 TaskLinkDrawingCallbackDelegate"
second_title: "Aspose.Tasks for .NET API 참조"
description: "작업 링크가 간트 차트 뷰에 렌더링될 때 호출되는 콜백을 나타냅니다."
type: docs
weight: 2240
url: /ko/net/aspose.tasks.saving/tasklinkdrawingcallbackdelegate/
---
## TaskLinkDrawingCallbackDelegate delegate

Gantt 차트 보기에서 작업 링크가 렌더링될 때 호출되는 콜백을 나타냅니다.

```csharp
public delegate void TaskLinkDrawingCallbackDelegate(TaskLinkDrawingArgs args);
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| args | TaskLinkDrawingArgs | 콜백 데이터를 포함하는 [`TaskLinkDrawingArgs`](../../aspose.tasks/tasklinkdrawingargs/) 클래스의 인스턴스입니다. |

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

* class [TaskLinkDrawingArgs](../../aspose.tasks/tasklinkdrawingargs/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


