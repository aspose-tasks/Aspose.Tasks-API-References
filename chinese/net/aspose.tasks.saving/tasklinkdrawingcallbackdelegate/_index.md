---
title: "委托 TaskLinkDrawingCallbackDelegate"
second_title: "Aspose.Tasks for .NET API 参考"
description: "表示在甘特图视图中渲染任务链接时调用的回调"
type: docs
weight: 2240
url: /zh/net/aspose.tasks.saving/tasklinkdrawingcallbackdelegate/
---
## TaskLinkDrawingCallbackDelegate delegate

表示在甘特图视图中渲染任务链接时调用的回调。

```csharp
public delegate void TaskLinkDrawingCallbackDelegate(TaskLinkDrawingArgs args);
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| args | TaskLinkDrawingArgs | 包含回调数据的[`TaskLinkDrawingArgs`](../../aspose.tasks/tasklinkdrawingargs/)类的实例。 |

## 示例

展示如何使用 TaskLinkDrawingCallback 在渲染甘特图视图时自定义任务链接的颜色。

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

### 另见

* class [TaskLinkDrawingArgs](../../aspose.tasks/tasklinkdrawingargs/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


