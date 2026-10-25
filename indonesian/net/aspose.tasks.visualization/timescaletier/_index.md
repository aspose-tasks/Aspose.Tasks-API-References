---
title: "Kelas TimescaleTier"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.TimescaleTier. Mewakili satu tingkat skala waktu pada Diagram Gantt"
type: docs
weight: 3450
url: /id/net/aspose.tasks.visualization/timescaletier/
---
## TimescaleTier class

Mewakili satu tingkatan skala waktu pada Gantt Chart.

```csharp
public sealed class TimescaleTier
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [TimescaleTier](timescaletier/#constructor)() | Menginisialisasi instance baru dari kelas `TimescaleTier`. |
| [TimescaleTier](timescaletier/#constructor_1)(TimescaleUnit, int) | Menginisialisasi instance baru dari kelas `TimescaleTier`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Alignment](../../aspose.tasks.visualization/timescaletier/alignment/) { get; set; } | Mendapatkan atau mengatur cara menyejajarkan label dalam setiap periode waktu tingkat ([`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [Count](../../aspose.tasks.visualization/timescaletier/count/) { get; set; } | Mendapatkan atau mengatur interval satuan waktu di mana label ditampilkan untuk tingkat. Nilai default adalah 1. |
| [DateTimeConverter](../../aspose.tasks.visualization/timescaletier/datetimeconverter/) { get; set; } | Mendapatkan atau mengatur fungsi callback untuk menangani rendering tanda tanggal pada tingkat ini. |
| [Label](../../aspose.tasks.visualization/timescaletier/label/) { get; set; } | Mendapatkan atau mengatur label tanggal [`DateLabel`](../datelabel/) untuk tingkat skala waktu. |
| [RenderLabelOnEachPage](../../aspose.tasks.visualization/timescaletier/renderlabeloneachpage/) { get; set; } | Mendapatkan atau mengatur flag yang menentukan apakah label tanggal harus dirender pada setiap halaman ketika periode waktu melintasi beberapa halaman. Jika nilai 'true', ketika periode waktu melintasi beberapa halaman, label tanggal untuk periode tersebut dirender pada setiap halaman. Jika nilai 'false', label tanggal dirender hanya sekali sesuai nilai properti [`Alignment`](./alignment/). |
| [ShowTicks](../../aspose.tasks.visualization/timescaletier/showticks/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan tanda centang yang memisahkan periode waktu dalam tingkat. |
| [Unit](../../aspose.tasks.visualization/timescaletier/unit/) { get; set; } | Mendapatkan atau mengatur satuan skala waktu [`TimescaleUnit`](../timescaleunit/) untuk tingkat skala waktu. Nilai default adalah [`Days`](../timescaleunit/). |
| [UsesFiscalYear](../../aspose.tasks.visualization/timescaletier/usesfiscalyear/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah label tingkat didasarkan pada tahun fiskal. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


