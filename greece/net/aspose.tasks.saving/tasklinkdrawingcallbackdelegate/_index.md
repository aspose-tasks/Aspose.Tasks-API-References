---
title: "Delegate TaskLinkDrawingCallbackDelegate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Αντιπροσωπεύει μια κλήση επιστροφής που καλείται όταν ένας σύνδεσμος εργασίας αποδίδεται σε προβολή γραφήματος Gantt"
type: docs
weight: 2240
url: /el/net/aspose.tasks.saving/tasklinkdrawingcallbackdelegate/
---
## TaskLinkDrawingCallbackDelegate delegate

Αντιπροσωπεύει μια κλήση επιστροφής που καλείται όταν ένας σύνδεσμος εργασίας αποδίδεται σε προβολή διαγράμματος Gantt.

```csharp
public delegate void TaskLinkDrawingCallbackDelegate(TaskLinkDrawingArgs args);
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| args | TaskLinkDrawingArgs | η παρουσία της κλάσης [`TaskLinkDrawingArgs`](../../aspose.tasks/tasklinkdrawingargs/) που περιέχει τα δεδομένα της κλήσης επιστροφής. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε το TaskLinkDrawingCallback για να προσαρμόσετε το χρώμα ενός συνδέσμου εργασίας κατά την απόδοση της προβολής γραφήματος Gantt.

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

### Δείτε επίσης

* class [TaskLinkDrawingArgs](../../aspose.tasks/tasklinkdrawingargs/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


