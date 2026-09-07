---
title: "SaveOptions.TimescaleFitBehavior"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur perilaku yang menentukan cara menyelaraskan ujung kanan skala waktu dengan ujung halaman"
type: docs
weight: 210
url: /id/net/aspose.tasks.saving/saveoptions/timescalefitbehavior/
---
## SaveOptions.TimescaleFitBehavior property

Mendapatkan atau mengatur perilaku yang menentukan cara menyelaraskan ujung kanan skala waktu dengan ujung halaman.

```csharp
public TimescaleFitBehavior TimescaleFitBehavior { get; set; }
```

## Contoh

Menampilkan cara menggunakan TimescaleFitBehavior agar skala waktu diagram Gantt menyesuaikan hingga akhir halaman terakhir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### Lihat Juga

* enum [TimescaleFitBehavior](../../../aspose.tasks.visualization/timescalefitbehavior/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


