---
title: "Delegado TaskLinkDrawingCallbackDelegate"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Representa una devolución de llamada que se invoca cuando se renderiza un enlace de tarea en una vista de diagrama de Gantt."
type: docs
weight: 2240
url: /es/net/aspose.tasks.saving/tasklinkdrawingcallbackdelegate/
---
## TaskLinkDrawingCallbackDelegate delegate

Representa una devolución de llamada que se invoca cuando se renderiza un enlace de tarea en una vista de diagrama de Gantt.

```csharp
public delegate void TaskLinkDrawingCallbackDelegate(TaskLinkDrawingArgs args);
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| args | TaskLinkDrawingArgs | la instancia de la clase [`TaskLinkDrawingArgs`](../../aspose.tasks/tasklinkdrawingargs/) que contiene los datos de la devolución de llamada. |

## Ejemplos

Muestra cómo usar TaskLinkDrawingCallback para personalizar el color de un enlace de tarea al renderizar la vista de diagrama de Gantt.

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

### Ver también

* class [TaskLinkDrawingArgs](../../aspose.tasks/tasklinkdrawingargs/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


