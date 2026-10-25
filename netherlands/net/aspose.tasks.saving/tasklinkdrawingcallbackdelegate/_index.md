---
title: "Delegate TaskLinkDrawingCallbackDelegate"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Stelt een callback voor die wordt aangeroepen wanneer een taakkoppeling wordt gerenderd in een Gantt‑diagramweergave."
type: docs
weight: 2240
url: /nl/net/aspose.tasks.saving/tasklinkdrawingcallbackdelegate/
---
## TaskLinkDrawingCallbackDelegate delegate

Stelt een callback voor die wordt aangeroepen wanneer een taaklink wordt gerenderd in een Gantt-diagramweergave.

```csharp
public delegate void TaskLinkDrawingCallbackDelegate(TaskLinkDrawingArgs args);
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| args | TaskLinkDrawingArgs | de instantie van de [`TaskLinkDrawingArgs`](../../aspose.tasks/tasklinkdrawingargs/)‑klasse die de callback‑gegevens bevat. |

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

* class [TaskLinkDrawingArgs](../../aspose.tasks/tasklinkdrawingargs/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


