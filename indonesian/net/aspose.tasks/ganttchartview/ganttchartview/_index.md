---
title: "GanttChartView.GanttChartView"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor GanttChartView. Menginisialisasi instance baru dari kelas GanttChartView"
type: docs
weight: 10
url: /id/net/aspose.tasks/ganttchartview/ganttchartview/
---
## GanttChartView constructor

Menginisialisasi instance baru dari kelas [`GanttChartView`](../).

```csharp
public GanttChartView()
```

## Contoh

Menampilkan cara memodifikasi tingkat skala waktu.

```csharp
var project = new Project();

// Inisialisasi Tampilan Gantt Chart
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// atur jumlah Skala Waktu
view.TopTimescaleTier.Count = 2;
view.TopTimescaleTier.Unit = TimescaleUnit.Quarters;
view.TopTimescaleTier.Label = DateLabel.QuarterQQyy;
view.TopTimescaleTier.ShowTicks = false;

view.MiddleTimescaleTier.Count = 2;
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
view.MiddleTimescaleTier.ShowTicks = false;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayDdd;
view.BottomTimescaleTier.Count = 2;
view.BottomTimescaleTier.ShowTicks = false;

// tambahkan Tampilan Gantt Chart ke proyek
project.Views.Add(view);

// tambahkan beberapa data uji ke proyek
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// Gunakan opsi 'Timescale.DefinedInView' untuk merender skala waktu menggunakan pengaturan skala waktu yang telah kami atur (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

### Lihat Juga

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


