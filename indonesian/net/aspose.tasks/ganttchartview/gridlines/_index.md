---
title: "GanttChartView.Gridlines"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti GanttChartView. Mendapatkan atau mengatur daftar Gridlines dari tampilan Gantt Chart"
type: docs
weight: 80
url: /id/net/aspose.tasks/ganttchartview/gridlines/
---
## GanttChartView.Gridlines property

Mendapatkan atau mengatur daftar `Gridlines` dari tampilan Gantt Chart.

```csharp
public List<Gridlines> Gridlines { get; set; }
```

## Contoh

Menampilkan cara bekerja dengan garis kisi.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var view = (GanttChartView)project.Views.ToList()[0];

// memungkinkan menyesuaikan garis kisi pertama pada tampilan
var gridlines = view.Gridlines[0];
// atur angka dari 0 hingga 99 yang menentukan interval antar garis kisi.
gridlines.Interval = 2;
// atur warna garis kisi sekunder.
gridlines.IntervalColor = Color.Red;
// atur pola garis untuk garis kisi sekunder
gridlines.IntervalPattern = LinePattern.Solid;
// atur warna garis kisi normal
gridlines.NormalColor = Color.Blue;
// atur pola garis untuk garis kisi normal
gridlines.NormalPattern = LinePattern.CloseDot;
// atur tipe garis kisi
gridlines.Type = GridlineType.GanttRow;

project.Save(OutDir + "WorkWithGridlines_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [Gridlines](../../../aspose.tasks.visualization/gridlines/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


