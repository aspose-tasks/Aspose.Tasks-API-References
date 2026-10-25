---
title: "GanttChartView.BarSize"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti GanttChartView. Mendapatkan atau mengatur tinggi dalam poin dari batang Gantt pada Gantt Chart"
type: docs
weight: 40
url: /id/net/aspose.tasks/ganttchartview/barsize/
---
## GanttChartView.BarSize property

Mendapatkan atau mengatur tinggi, dalam poin, dari batang Gantt dalam Gantt Chart.

```csharp
public GanttBarSize BarSize { get; set; }
```

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

* enum [GanttBarSize](../../ganttbarsize/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


