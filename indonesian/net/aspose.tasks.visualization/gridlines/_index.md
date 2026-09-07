---
title: "Class Gridlines"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.Visualization.Gridlines class. Mewakili garis kisi yang muncul dalam tampilan GanttChart."
type: docs
weight: 3120
url: /id/net/aspose.tasks.visualization/gridlines/
---
## Gridlines class

Mewakili garis kisi yang muncul dalam tampilan GanttChart.

```csharp
public class Gridlines
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Gridlines](gridlines/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Interval](../../aspose.tasks.visualization/gridlines/interval/) { get; set; } | Mendapatkan atau mengatur angka dari 0 hingga 99 yang menentukan interval antara garis kisi. |
| [IntervalColor](../../aspose.tasks.visualization/gridlines/intervalcolor/) { get; set; } | Mendapatkan atau mengatur warna garis kisi sekunder. |
| [IntervalPattern](../../aspose.tasks.visualization/gridlines/intervalpattern/) { get; set; } | Mendapatkan atau mengatur pola garis untuk garis kisi sekunder. |
| [NormalColor](../../aspose.tasks.visualization/gridlines/normalcolor/) { get; set; } | Mendapatkan atau mengatur warna garis kisi normal. |
| [NormalPattern](../../aspose.tasks.visualization/gridlines/normalpattern/) { get; set; } | Mendapatkan atau mengatur pola garis untuk garis kisi normal. |
| [Type](../../aspose.tasks.visualization/gridlines/type/) { get; set; } | Mendapatkan atau mengatur tipe garis kisi. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


