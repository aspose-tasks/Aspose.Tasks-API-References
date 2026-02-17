---
title: Delegate TaskLinkDrawingCallbackDelegate
second_title: Aspose.Tasks for .NET API Reference
description: Represents a callback that is called when a task link is rendered in a Gantt chart view
type: docs
weight: 2220
url: /net/aspose.tasks.saving/tasklinkdrawingcallbackdelegate/
---
## TaskLinkDrawingCallbackDelegate delegate

Represents a callback that is called when a task link is rendered in a Gantt chart view.

```csharp
public delegate void TaskLinkDrawingCallbackDelegate(TaskLinkDrawingArgs args);
```

| Parameter | Type | Description |
| --- | --- | --- |
| args | TaskLinkDrawingArgs | the instance of the [`TaskLinkDrawingArgs`](../../aspose.tasks/tasklinkdrawingargs/) class that contains the callback data. |

## Examples

Shows how to use TaskLinkDrawingCallback to customize color of a task link when rendering Gantt chart view.

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

### See Also

* class [TaskLinkDrawingArgs](../../aspose.tasks/tasklinkdrawingargs/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


