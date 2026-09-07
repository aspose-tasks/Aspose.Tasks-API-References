---
title: "Kelas ProgressLines"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.ProgressLines. Mewakili garis kemajuan dalam tampilan Gantt Chart."
type: docs
weight: 3290
url: /id/net/aspose.tasks.visualization/progresslines/
---
## ProgressLines class

Mewakili garis kemajuan dalam tampilan Gantt Chart.

```csharp
public class ProgressLines
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [ProgressLines](progresslines/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [BeginAtDate](../../aspose.tasks.visualization/progresslines/beginatdate/) { get; set; } | Mendapatkan atau mengatur tanggal untuk menampilkan garis kemajuan mulai dari. |
| [BeginAtProjectStart](../../aspose.tasks.visualization/progresslines/beginatprojectstart/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan garis kemajuan sejak awal tanggal mulai proyek. |
| [DateFormat](../../aspose.tasks.visualization/progresslines/dateformat/) { get; set; } | Mendapatkan atau mengatur format tanggal ([`DateLabel`](../datelabel/)). |
| [DisplayAtCurrentDate](../../aspose.tasks.visualization/progresslines/displayatcurrentdate/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan garis kemajuan pada tanggal saat ini. |
| [DisplayAtRecurringIntervals](../../aspose.tasks.visualization/progresslines/displayatrecurringintervals/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan garis kemajuan pada interval berulang. |
| [DisplaySelected](../../aspose.tasks.visualization/progresslines/displayselected/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan garis kemajuan pada tanggal yang dipilih. |
| [Font](../../aspose.tasks.visualization/progresslines/font/) { get; set; } | Mendapatkan atau mengatur font yang digunakan untuk label garis kemajuan. |
| [IsBaselinePlan](../../aspose.tasks.visualization/progresslines/isbaselineplan/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan garis kemajuan untuk rencana dasar atau aktual. |
| [LineColor](../../aspose.tasks.visualization/progresslines/linecolor/) { get; set; } | Mendapatkan atau mengatur warna garis untuk garis kemajuan saat ini. |
| [LinePattern](../../aspose.tasks.visualization/progresslines/linepattern/) { get; set; } | Mendapatkan atau mengatur pola garis dari garis kemajuan saat ini. [`LinePattern`](./linepattern/). |
| [OtherLineColor](../../aspose.tasks.visualization/progresslines/otherlinecolor/) { get; set; } | Mendapatkan atau mengatur warna garis kemajuan lainnya. |
| [OtherLinePattern](../../aspose.tasks.visualization/progresslines/otherlinepattern/) { get; set; } | Mendapatkan atau mengatur pola garis untuk garis kemajuan lainnya. |
| [OtherProgressPointColor](../../aspose.tasks.visualization/progresslines/otherprogresspointcolor/) { get; set; } | Mendapatkan atau mengatur warna titik kemajuan lainnya. |
| [OtherProgressPointShape](../../aspose.tasks.visualization/progresslines/otherprogresspointshape/) { get; set; } | Mendapatkan atau mengatur bentuk titik kemajuan dari garis kemajuan lainnya. |
| [ProgressPointColor](../../aspose.tasks.visualization/progresslines/progresspointcolor/) { get; set; } | Mendapatkan atau mengatur warna titik kemajuan. |
| [ProgressPointShape](../../aspose.tasks.visualization/progresslines/progresspointshape/) { get; set; } | Mendapatkan atau mengatur bentuk titik kemajuan. [`GanttBarEndShape`](../ganttbarendshape/). |
| [RecurringInterval](../../aspose.tasks.visualization/progresslines/recurringinterval/) { get; set; } | Mendapatkan atau mengatur interval berulang. [`RecurringInterval`](./recurringinterval/). |
| [SelectedDates](../../aspose.tasks.visualization/progresslines/selecteddates/) { get; } | Mendapatkan daftar tanggal yang dipilih untuk menampilkan garis kemajuan. |
| [ShowDate](../../aspose.tasks.visualization/progresslines/showdate/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan tanggal untuk setiap garis kemajuan. |

## Contoh

Menampilkan cara bekerja dengan garis kemajuan.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// mari definisikan garis kemajuan
view.ProgressLines = new ProgressLines();
var progressLines = view.ProgressLines;

// atur tanggal untuk menampilkan garis kemajuan mulai dari. Mari atur tanggal status proyek.
progressLines.BeginAtDate = project.Get(Prj.StatusDate);
// atur nilai yang menunjukkan apakah menampilkan garis kemajuan sejak tanggal mulai proyek
progressLines.BeginAtProjectStart = true;
// atur format tanggal (<see cref="T:Aspose.Tasks.Visualization.DateLabel" />).
progressLines.DateFormat = DateLabel.DayDddd;
// atur nilai yang menunjukkan apakah menampilkan garis kemajuan pada tanggal saat ini.
progressLines.DisplayAtCurrentDate = true;
// atur nilai yang menunjukkan apakah menampilkan garis kemajuan pada interval berulang.
progressLines.DisplayAtRecurringIntervals = true;
// atur nilai yang menunjukkan apakah menampilkan garis kemajuan pada tanggal yang dipilih
progressLines.DisplaySelected = true;
// atur nilai yang menunjukkan apakah menampilkan garis kemajuan untuk rencana baseline atau aktual.
progressLines.IsBaselinePlan = false;
// atur font yang digunakan untuk label garis kemajuan.
progressLines.Font = new FontDescriptor("Arial", 10);
// atur warna garis untuk garis kemajuan saat ini.
progressLines.LineColor = Color.Aquamarine;
// atur pola garis dari garis kemajuan saat ini.
progressLines.LinePattern = LinePattern.Dashed;
// atur warna garis kemajuan lainnya.
progressLines.OtherLineColor = Color.Azure;
// atur pola garis untuk garis kemajuan lainnya.
progressLines.OtherLinePattern = LinePattern.Dotted;
// atur warna titik kemajuan lainnya.
progressLines.OtherProgressPointColor = Color.Red;
// atur bentuk titik kemajuan dari garis kemajuan lainnya.
progressLines.OtherProgressPointShape = GanttBarEndShape.Circle;
// atur warna titik kemajuan.
progressLines.ProgressPointColor = Color.Orange;
// atur bentuk titik kemajuan.
progressLines.ProgressPointShape = GanttBarEndShape.Diamond;
// atur interval berulang.
progressLines.RecurringInterval = new RecurringInterval();
// atur interval berulang.
progressLines.RecurringInterval.Interval = Interval.Daily;
// atur nomor hari harian
progressLines.RecurringInterval.DailyDayNumber = 1;
// atur nilai yang menunjukkan apakah menampilkan tanggal untuk setiap baris kemajuan.
progressLines.ShowDate = true;

// mari periksa baris kemajuan
Console.WriteLine("Begin At Date: " + progressLines.BeginAtDate);
Console.WriteLine("Begin At Project Start: " + progressLines.BeginAtProjectStart);
Console.WriteLine("Date Format: " + progressLines.DateFormat);
Console.WriteLine("Display At Current Date: " + progressLines.DisplayAtCurrentDate);
Console.WriteLine("Display At Recurring Intervals: " + progressLines.DisplayAtRecurringIntervals);
Console.WriteLine("Display Selected: " + progressLines.DisplaySelected);
Console.WriteLine("Font: " + progressLines.Font);
Console.WriteLine("Is Baseline Plan: " + progressLines.IsBaselinePlan);
Console.WriteLine("Line Color: " + progressLines.LineColor);
Console.WriteLine("Line Pattern: " + progressLines.LinePattern);
Console.WriteLine("Other Line Color: " + progressLines.OtherLineColor);
Console.WriteLine("Other Line Pattern: " + progressLines.OtherLinePattern);
Console.WriteLine("Other Progress Point Color: " + progressLines.OtherProgressPointColor);
Console.WriteLine("Other Progress Point Shape: " + progressLines.OtherProgressPointShape);
Console.WriteLine("Progress Point Color: " + progressLines.ProgressPointColor);
Console.WriteLine("Progress Point Shape: " + progressLines.ProgressPointShape);
Console.WriteLine("Recurring Interval: " + progressLines.RecurringInterval.Interval);
Console.WriteLine("Recurring Interval DailyDayNumber: " + progressLines.RecurringInterval.DailyDayNumber);
Console.WriteLine("Selected Dates: ");
foreach (var date in progressLines.SelectedDates)
{
    Console.WriteLine("Date: " + date);
}
Console.WriteLine("Show Date: " + progressLines.ShowDate);
Console.WriteLine();

project.Save(OutDir + "WorkWithProgressLines_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


