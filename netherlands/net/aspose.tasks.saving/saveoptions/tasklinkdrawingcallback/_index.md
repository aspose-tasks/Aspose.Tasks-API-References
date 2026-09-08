---
title: "SaveOptions.TaskLinkDrawingCallback"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions eigenschap. Haalt een callback op of stelt deze in die kan worden gebruikt om enkele aspecten van het renderen van taakkoppelingen aan te passen"
type: docs
weight: 180
url: /nl/net/aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/
---
## SaveOptions.TaskLinkDrawingCallback property

Haalt op of stelt een callback in die kan worden gebruikt om enkele aspecten van het renderen van taakkoppelingen aan te passen.

```csharp
public TaskLinkDrawingCallbackDelegate TaskLinkDrawingCallback { get; set; }
```

## Opmerkingen

Is alleen van toepassing wanneer de Gantt‑chartweergave wordt gerenderd.

## Voorbeelden

Toont hoe TaskLinkDrawingCallback te gebruiken om de kleur van een taakkoppeling aan te passen bij het renderen van een Gantt‑diagramweergave.

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

### Zie ook

* delegate [TaskLinkDrawingCallbackDelegate](../../tasklinkdrawingcallbackdelegate/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


