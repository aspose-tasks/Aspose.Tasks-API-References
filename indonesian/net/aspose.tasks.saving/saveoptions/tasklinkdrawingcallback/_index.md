---
title: "SaveOptions.TaskLinkDrawingCallback"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur callback yang dapat digunakan untuk menyesuaikan beberapa aspek rendering tautan tugas"
type: docs
weight: 180
url: /id/net/aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/
---
## SaveOptions.TaskLinkDrawingCallback property

Mendapatkan atau mengatur callback yang dapat digunakan untuk menyesuaikan beberapa aspek rendering tautan tugas.

```csharp
public TaskLinkDrawingCallbackDelegate TaskLinkDrawingCallback { get; set; }
```

## Catatan

Hanya berlaku ketika tampilan diagram Gantt dirender.

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

* delegate [TaskLinkDrawingCallbackDelegate](../../tasklinkdrawingcallbackdelegate/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


