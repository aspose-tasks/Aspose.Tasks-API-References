---
title: "SaveOptions.LegendDrawingOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur nilai yang menentukan bagaimana merender legenda. Nilai default adalah LegendDrawingOptions.OnEveryPage"
type: docs
weight: 80
url: /id/net/aspose.tasks.saving/saveoptions/legenddrawingoptions/
---
## SaveOptions.LegendDrawingOptions property

Mendapatkan atau mengatur nilai yang menentukan cara merender legenda. Nilai default adalah LegendDrawingOptions.OnEveryPage.

```csharp
public LegendDrawingOptions LegendDrawingOptions { get; set; }
```

## Catatan

Hanya berlaku ketika tampilan diagram Gantt dirender.

## Contoh

Menampilkan cara mencetak legenda pada halaman terakhir

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Ambil opsi gambar legenda dari tampilan
    LegendDrawingOptions = LegendDrawingOptions.AfterLastPage
};

project.Save(OutDir + "LegendOnSeparatePage_out.pdf", options);
```

Menampilkan cara menyembunyikan legenda halaman.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Tentukan LegendDrawingOptions.NoLegend untuk menyembunyikan legenda
    LegendDrawingOptions = LegendDrawingOptions.NoLegend
};

project.Save(OutDir + "HideLegendsDuringSave_out.pdf", options);
```

Menampilkan cara menggunakan opsi LegendDrawingOptions.DefinedInView.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var view = project.Views.GetByName("&Gantt Chart");

Console.WriteLine("LegendOn option defined in view '{0}': {1}", view.Name, view.PageInfo.Legend.LegendOn);

SaveOptions options = new PdfSaveOptions
{
    // Ambil opsi gambar legenda dari tampilan
    LegendDrawingOptions = LegendDrawingOptions.DefinedInView,
    ViewSettings = view
};

project.Save(OutDir + "Legend_DefinedInView.pdf", options);
```

Menampilkan cara menyesuaikan batang tugas dalam legenda halaman pada diagram Gantt.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.StartDate = project.StartDate;
pdfSaveOptions.EndDate = project.FinishDate;
pdfSaveOptions.PageSize = PageSize.A4;
pdfSaveOptions.LegendDrawingOptions = LegendDrawingOptions.OnEveryPage;
pdfSaveOptions.ViewSettings = project.Views.GetByName("&Gantt Chart");

pdfSaveOptions.LegendItems = new PageLegendItem[]
{
    new PageLegendItem(BarItemType.Task, "Task"),
    new PageLegendItem(BarItemType.ExternalMilestone, "External Milestone"),
    new PageLegendItem(BarItemType.SummaryRollup, "Summary Rollup"),
    new PageLegendItem(BarItemType.InactiveTask, "Inactive Task"),
    new PageLegendItem(BarItemType.ManualSummary, "Manual Summary")
};

project.Save(OutDir + "CustomizePageLegendItems_out.pdf", pdfSaveOptions);
```

### Lihat Juga

* enum [LegendDrawingOptions](../../legenddrawingoptions/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


