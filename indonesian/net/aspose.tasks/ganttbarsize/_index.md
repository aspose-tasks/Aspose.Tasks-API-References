---
title: "Enum GanttBarSize"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.GanttBarSize enum. Menentukan tinggi bar dalam poin"
type: docs
weight: 700
url: /id/net/aspose.tasks/ganttbarsize/
---
## GanttBarSize enumeration

Menentukan tinggi bar dalam poin.

```csharp
public enum GanttBarSize
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| BarSize6 | `0` | Ukuran bar 6 poin. |
| BarSize8 | `1` | Ukuran bar 8 poin. |
| BarSize10 | `2` | Ukuran bar 10 poin. |
| BarSize12 | `3` | Ukuran bar 12 poin. |
| BarSize14 | `4` | Ukuran bar 14 poin. |
| BarSize18 | `5` | Ukuran bar 18 poin. |
| BarSize24 | `6` | Ukuran bar 24 poin. |

## Contoh

Menampilkan cara mengatur beberapa properti berguna dari tampilan diagram Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// atur nilai yang menunjukkan apakah bar dibulatkan ke hari terdekat
view.BarRounding = false;
// atur tinggi, dalam poin, dari bar Gantt dalam Diagram Gantt
view.BarSize = GanttBarSize.BarSize24;
// atur nilai yang menunjukkan apakah bar rollup akan disembunyikan saat memperluas tugas rangkuman
view.HideRollupBarsWhenSummaryExpanded = true;
// atur warna waktu non-kerja
view.NonWorkingTimeColor = Color.Azure;
// atur nilai yang menunjukkan apakah bar pada Diagram Gantt harus digulung
view.RollUpGanttBars = true;
// atur nilai yang menunjukkan apakah pemisahan tugas pada Diagram Gantt harus ditampilkan
view.ShowBarSplits = true;
// atur nilai yang menunjukkan apakah gambar pada Diagram Gantt harus ditampilkan
view.ShowDrawings = true;
// atur persentase untuk mengurangi atau memperbesar jarak antar unit pada tingkat skala waktu
view.TimescaleSizePercentage = 10;

project.Save(OutDir + "WorkWithGanttChartViews_out.pdf", SaveFileFormat.Pdf);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


