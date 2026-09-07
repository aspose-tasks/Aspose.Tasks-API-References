---
title: "GanttChartView.MiddleTimescaleTier"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti GanttChartView. Mendapatkan atau mengatur pengaturan tier skala waktu tengah tampilan. TimescaleTier"
type: docs
weight: 100
url: /id/net/aspose.tasks/ganttchartview/middletimescaletier/
---
## GanttChartView.MiddleTimescaleTier property

Mendapatkan atau mengatur pengaturan tier skala waktu menengah tampilan. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier MiddleTimescaleTier { get; set; }
```

## Contoh

Menampilkan cara bekerja dengan tier skala waktu melalui opsi penyimpanan.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

GanttChartView ganttChartView = (GanttChartView) project.Views.ToList()[0];

// atur tier skala waktu tampilan Gantt Chart
ganttChartView.MiddleTimescaleTier.Unit = TimescaleUnit.Months;
ganttChartView.MiddleTimescaleTier.Count = 1;
ganttChartView.MiddleTimescaleTier.Label = DateLabel.MonthMmmm;

ganttChartView.BottomTimescaleTier.Unit = TimescaleUnit.Days;
ganttChartView.BottomTimescaleTier.Count = 1;
ganttChartView.BottomTimescaleTier.Label = DateLabel.DayDddDd;

// ...
var options = new ImageSaveOptions(SaveFileFormat.Png)
{
    Timescale = Timescale.DefinedInView
};

// ...

// simpan proyek sebagai gambar
project.Save(OutDir + "WorkWithTimescaleTier_out.png", options);
```

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

Menampilkan cara menyesuaikan label tingkat skala waktu.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Tambahkan tautan tugas
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// sesuaikan tingkat skala waktu

// sesuaikan tingkat atas
// atur tingkat skala waktu atas pada tampilan Diagram Gantt.
view.MiddleTimescaleTier = new TimescaleTier();
// atur satuan skala waktu <see cref=\"T:Aspose.Tasks.Visualization.TimescaleUnit\" /> untuk tingkat skala waktu.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// atur interval satuan waktu di mana label ditampilkan untuk tingkat.
view.MiddleTimescaleTier.Count = 1;
// atur label tanggal <see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" /> untuk tingkat skala waktu.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// atur cara menyejajarkan label dalam setiap periode waktu tingkat (<see cref=\"T:System.Drawing.StringAlignment\" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// atur nilai yang menunjukkan apakah menampilkan tanda centang yang memisahkan periode waktu dalam tingkat.
view.MiddleTimescaleTier.ShowTicks = true;
// atur nilai yang menunjukkan apakah mendasarkan label tingkat pada tahun fiskal.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// ditambahkan untuk visualisasi yang lebih baik
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// sesuaikan tanggal tingkat tengah
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Gunakan opsi 'Timescale.DefinedInView' untuk merender skala waktu menggunakan pengaturan skala waktu yang didefinisikan dalam tampilan (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### Lihat Juga

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


