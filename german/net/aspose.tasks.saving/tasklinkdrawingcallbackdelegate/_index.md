---
title: "Delegate TaskLinkDrawingCallbackDelegate"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Stellt einen Rückruf dar, der aufgerufen wird, wenn ein Aufgabenlink in einer Gantt‑Diagrammansicht gerendert wird"
type: docs
weight: 2240
url: /de/net/aspose.tasks.saving/tasklinkdrawingcallbackdelegate/
---
## TaskLinkDrawingCallbackDelegate delegate

Stellt einen Rückruf dar, der aufgerufen wird, wenn ein Aufgabenlink in einer Gantt‑Diagrammansicht gerendert wird.

```csharp
public delegate void TaskLinkDrawingCallbackDelegate(TaskLinkDrawingArgs args);
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| args | TaskLinkDrawingArgs | die Instanz der [`TaskLinkDrawingArgs`](../../aspose.tasks/tasklinkdrawingargs/) Klasse, die die Rückrufdaten enthält. |

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

* class [TaskLinkDrawingArgs](../../aspose.tasks/tasklinkdrawingargs/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


