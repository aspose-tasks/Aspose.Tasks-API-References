---
title: "SaveOptions.RollUpGanttBars"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah subtugas pada bar tugas ringkasan harus ditandai. Untuk subtugas, bidang Rollup menunjukkan apakah informasi pada bar Gantt subtugas akan digabungkan ke bar tugas ringkasan. Untuk tugas ringkasan, bidang Rollup menunjukkan apakah bar tugas ringkasan menampilkan bar yang digabungkan. Anda harus mengatur bidang Rollup untuk tugas ringkasan ke Ya agar subtugas apa pun dapat digabungkan ke dalamnya."
type: docs
weight: 160
url: /id/net/aspose.tasks.saving/saveoptions/rollupganttbars/
---
## SaveOptions.RollUpGanttBars property

Mendapatkan atau mengatur nilai yang menunjukkan apakah subtugas pada batang tugas ringkasan harus ditandai. Untuk subtugas, bidang Rollup menunjukkan apakah informasi pada batang Gantt subtugas akan digabungkan ke batang tugas ringkasan. Untuk tugas ringkasan, bidang Rollup menunjukkan apakah batang tugas ringkasan menampilkan batang yang digabungkan. Anda harus mengatur bidang Rollup untuk tugas ringkasan ke Ya agar subtugas apa pun dapat digabungkan ke dalamnya.

```csharp
public bool RollUpGanttBars { get; set; }
```

## Catatan

Hanya berlaku ketika tampilan diagram Gantt dirender.

## Contoh

Menampilkan cara mengatur nilai yang menunjukkan bahwa subtugas pada bar tugas rangkuman harus digulung naik.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // ATAU
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### Lihat Juga

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


