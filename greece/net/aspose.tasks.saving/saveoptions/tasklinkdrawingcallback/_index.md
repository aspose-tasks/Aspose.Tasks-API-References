---
title: "SaveOptions.TaskLinkDrawingCallback"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει μια κλήση επιστροφής (callback) που μπορεί να χρησιμοποιηθεί για την προσαρμογή ορισμένων πτυχών της απόδοσης των συνδέσμων εργασιών."
type: docs
weight: 180
url: /el/net/aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/
---
## SaveOptions.TaskLinkDrawingCallback property

Λαμβάνει ή ορίζει μια κλήση επιστροφής που μπορεί να χρησιμοποιηθεί για την προσαρμογή ορισμένων πτυχών της απόδοσης συνδέσμων εργασιών.

```csharp
public TaskLinkDrawingCallbackDelegate TaskLinkDrawingCallback { get; set; }
```

## Παρατηρήσεις

Ισχύει μόνο όταν η προβολή Gantt chart αποδίδεται.

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

* delegate [TaskLinkDrawingCallbackDelegate](../../tasklinkdrawingcallbackdelegate/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


