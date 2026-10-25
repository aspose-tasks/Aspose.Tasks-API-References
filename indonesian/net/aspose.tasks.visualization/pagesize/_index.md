---
title: "Enum PageSize"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.Visualization.PageSize enum. Menentukan ukuran halaman"
type: docs
weight: 3250
url: /id/net/aspose.tasks.visualization/pagesize/
---
## PageSize enumeration

Menentukan ukuran halaman.

```csharp
public enum PageSize
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Letter | `0` | Ukuran halaman Letter dalam poin adalah 792 × 612 |
| Ledger | `1` | Ukuran halaman Ledger dalam poin adalah 1224 × 792 |
| A0 | `2` | Ukuran halaman A0 dalam poin adalah 3371 × 2384 |
| A1 | `3` | Ukuran halaman A1 dalam poin adalah 2384 × 1685 |
| A2 | `4` | Ukuran halaman A2 dalam poin adalah 1684 × 1190 |
| A3 | `5` | Ukuran halaman A3 dalam poin adalah 1190 × 842 |
| A4 | `6` | Ukuran halaman A4 dalam poin adalah 842 × 595 |
| DefinedInView | `7` | Gunakan ukuran halaman yang didefinisikan dalam View's [`PageSettings`](../pagesettings/) (View.PageInfo.PageSettings). |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


