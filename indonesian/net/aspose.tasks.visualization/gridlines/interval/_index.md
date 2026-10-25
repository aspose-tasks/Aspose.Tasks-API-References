---
title: "Gridlines.Interval"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Gridlines. Mendapatkan atau mengatur angka dari 0 hingga 99 yang menentukan interval antar garis kisi"
type: docs
weight: 20
url: /id/net/aspose.tasks.visualization/gridlines/interval/
---
## Gridlines.Interval property

Mendapatkan atau mengatur angka dari 0 hingga 99 yang menentukan interval antara garis kisi.

```csharp
public int Interval { get; set; }
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

* class [Gridlines](../)
* namespace [Aspose.Tasks.Visualization](../../gridlines/)
* assembly [Aspose.Tasks](../../../)


