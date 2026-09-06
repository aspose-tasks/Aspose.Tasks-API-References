---
title: "Delegate TaskLinkDrawingCallbackDelegate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Représente un rappel qui est appelé lorsqu'un lien de tâche est rendu dans une vue de diagramme de Gantt"
type: docs
weight: 2240
url: /fr/net/aspose.tasks.saving/tasklinkdrawingcallbackdelegate/
---
## TaskLinkDrawingCallbackDelegate delegate

Représente un rappel qui est appelé lorsqu'un lien de tâche est rendu dans une vue de diagramme de Gantt.

```csharp
public delegate void TaskLinkDrawingCallbackDelegate(TaskLinkDrawingArgs args);
```

| Paramètre | Type | Description |
| --- | --- | --- |
| args | TaskLinkDrawingArgs | l'instance de la classe [`TaskLinkDrawingArgs`](../../aspose.tasks/tasklinkdrawingargs/) qui contient les données du rappel. |

## Exemples

Montre comment utiliser TaskLinkDrawingCallback pour personnaliser la couleur d'un lien de tâche lors du rendu de la vue du diagramme de Gantt.

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

### Voir aussi

* class [TaskLinkDrawingArgs](../../aspose.tasks/tasklinkdrawingargs/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


