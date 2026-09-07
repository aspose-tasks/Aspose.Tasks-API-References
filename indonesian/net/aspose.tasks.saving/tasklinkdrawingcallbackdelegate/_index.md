---
title: "Delegate TaskLinkDrawingCallbackDelegate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Mewakili callback yang dipanggil ketika tautan tugas dirender dalam tampilan diagram Gantt"
type: docs
weight: 2240
url: /id/net/aspose.tasks.saving/tasklinkdrawingcallbackdelegate/
---
## TaskLinkDrawingCallbackDelegate delegate

Mewakili callback yang dipanggil ketika tautan tugas dirender dalam tampilan diagram Gantt.

```csharp
public delegate void TaskLinkDrawingCallbackDelegate(TaskLinkDrawingArgs args);
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| args | TaskLinkDrawingArgs | instance dari kelas [`TaskLinkDrawingArgs`](../../aspose.tasks/tasklinkdrawingargs/) yang berisi data callback. |

## Contoh

Menampilkan cara menggunakan TaskLinkDrawingCallback untuk menyesuaikan warna tautan tugas saat merender tampilan diagram Gantt.

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

### Lihat Juga

* class [TaskLinkDrawingArgs](../../aspose.tasks/tasklinkdrawingargs/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


