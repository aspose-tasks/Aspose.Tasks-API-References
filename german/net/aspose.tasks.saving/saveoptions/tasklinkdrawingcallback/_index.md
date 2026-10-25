---
title: "SaveOptions.TaskLinkDrawingCallback"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "SaveOptions‑Eigenschaft. Lässt einen Callback zu, der verwendet werden kann, um einige Aspekte der Darstellung von Aufgabenverknüpfungen anzupassen."
type: docs
weight: 180
url: /de/net/aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/
---
## SaveOptions.TaskLinkDrawingCallback property

Liest oder setzt einen Callback, der verwendet werden kann, um einige Aspekte der Darstellung von Aufgabenverknüpfungen anzupassen.

```csharp
public TaskLinkDrawingCallbackDelegate TaskLinkDrawingCallback { get; set; }
```

## Hinweise

Gilt nur, wenn die Gantt‑Diagrammansicht gerendert wird.

## Beispiele

Zeigt, wie TaskLinkDrawingCallback verwendet wird, um die Farbe eines Aufgabenlinks beim Rendern einer Gantt‑Diagrammansicht anzupassen.

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

### Siehe auch

* delegate [TaskLinkDrawingCallbackDelegate](../../tasklinkdrawingcallbackdelegate/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


