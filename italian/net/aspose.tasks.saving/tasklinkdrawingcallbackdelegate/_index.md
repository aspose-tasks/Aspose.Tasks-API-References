---
title: "Delegate TaskLinkDrawingCallbackDelegate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Rappresenta una callback che viene chiamata quando un collegamento tra attività viene renderizzato in una vista diagramma di Gantt"
type: docs
weight: 2240
url: /it/net/aspose.tasks.saving/tasklinkdrawingcallbackdelegate/
---
## TaskLinkDrawingCallbackDelegate delegate

Rappresenta un callback che viene chiamato quando un collegamento di attività viene renderizzato in una vista diagramma di Gantt.

```csharp
public delegate void TaskLinkDrawingCallbackDelegate(TaskLinkDrawingArgs args);
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| args | TaskLinkDrawingArgs | l'istanza della classe [`TaskLinkDrawingArgs`](../../aspose.tasks/tasklinkdrawingargs/) che contiene i dati della callback. |

## Esempi

Mostra come utilizzare TaskLinkDrawingCallback per personalizzare il colore di un collegamento tra attività durante il rendering della vista diagramma di Gantt.

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

### Vedi anche

* class [TaskLinkDrawingArgs](../../aspose.tasks/tasklinkdrawingargs/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


