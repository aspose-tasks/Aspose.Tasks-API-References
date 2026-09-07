---
title: "TimescaleTier.Unit"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "TimescaleTier properti. Mendapatkan atau mengatur satuan skala waktu TimescaleUnit untuk tier skala waktu. Nilai default adalah Days"
type: docs
weight: 80
url: /id/net/aspose.tasks.visualization/timescaletier/unit/
---
## TimescaleTier.Unit property

Mendapatkan atau mengatur satuan skala waktu [`TimescaleUnit`](../../timescaleunit/) untuk tier skala waktu. Nilai default adalah [`Days`](../../timescaleunit/).

```csharp
public TimescaleUnit Unit { get; set; }
```

## Contoh

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

* enum [TimescaleUnit](../../timescaleunit/)
* class [TimescaleTier](../)
* namespace [Aspose.Tasks.Visualization](../../timescaletier/)
* assembly [Aspose.Tasks](../../../)


