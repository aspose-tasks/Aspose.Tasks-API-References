---
title: "SaveOptions.DrawNonWorkingTime"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah waktu non‑kerja harus digambar. Nilai default adalah TRUE."
type: docs
weight: 30
url: /id/net/aspose.tasks.saving/saveoptions/drawnonworkingtime/
---
## SaveOptions.DrawNonWorkingTime property

Mendapatkan atau mengatur nilai yang menunjukkan apakah waktu non‑kerja harus digambar (Nilai default adalah TRUE).

```csharp
public bool DrawNonWorkingTime { get; set; }
```

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


