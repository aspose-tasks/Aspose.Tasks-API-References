---
title: "Kelas RecurringInterval"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.RecurringInterval. Mewakili interval berulang yang digunakan dalam garis kemajuan tampilan Gantt Chart"
type: docs
weight: 3310
url: /id/net/aspose.tasks.visualization/recurringinterval/
---
## RecurringInterval class

Mewakili interval berulang yang digunakan dalam garis kemajuan pada tampilan Gantt Chart.

```csharp
public class RecurringInterval
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [RecurringInterval](recurringinterval/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [DailyDayNumber](../../aspose.tasks.visualization/recurringinterval/dailydaynumber/) { get; set; } | Mendapatkan atau mengatur nomor hari harian. |
| [DailyWorkday](../../aspose.tasks.visualization/recurringinterval/dailyworkday/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah hari tersebut adalah hari kerja untuk garis kemajuan harian. |
| [Interval](../../aspose.tasks.visualization/recurringinterval/interval/) { get; set; } | Mendapatkan atau mengatur interval berulang. Dapat berupa nilai apa pun dari tipe [`Interval`](./interval/). |
| [MonthlyDay](../../aspose.tasks.visualization/recurringinterval/monthlyday/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan garis kemajuan bulanan per hari. |
| [MonthlyDayDayNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaydaynumber/) { get; set; } | Mendapatkan atau mengatur nomor hari dari garis kemajuan bulanan. |
| [MonthlyDayMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/) { get; set; } | Mendapatkan atau mengatur nomor bulan dari garis kemajuan bulanan. |
| [MonthlyFirstLast](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlast/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan garis kemajuan berdasarkan hari pertama atau terakhir yang telah ditentukan. |
| [MonthlyFirstLastDay](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastday/) { get; set; } | Mendapatkan atau mengatur tipe hari pertama atau terakhir dari garis kemajuan bulanan. |
| [MonthlyFirstLastMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastmonthnumber/) { get; set; } | Mendapatkan atau mengatur nomor bulan dari garis kemajuan, yang ditampilkan berdasarkan hari pertama atau terakhir yang telah ditentukan. |
| [WeeklyDays](../../aspose.tasks.visualization/recurringinterval/weeklydays/) { get; } | Mendapatkan daftar hari untuk garis kemajuan mingguan. |
| [WeeklyWeekNumber](../../aspose.tasks.visualization/recurringinterval/weeklyweeknumber/) { get; set; } | Mendapatkan atau mengatur nomor minggu untuk garis kemajuan mingguan. |

## Contoh

Menampilkan cara bekerja dengan interval berulang dari garis kemajuan.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

// memungkinkan membaca garis kemajuan
var interval = view.ProgressLines.RecurringInterval;

Console.WriteLine("Interval: " + interval.Interval);
Console.WriteLine("Weekly Week Number: " + interval.WeeklyWeekNumber);
foreach (var day in interval.WeeklyDays)
{
    Console.WriteLine("Week day: " + day);
}

// memungkinkan mendefinisikan ulang interval berulang
var newInterval = new RecurringInterval();

// menetapkan nilai yang menunjukkan apakah menampilkan garis kemajuan bulanan per hari.
interval.MonthlyDay = true;
// menetapkan nomor hari untuk garis kemajuan bulanan.
interval.MonthlyDayDayNumber = 1;
// menetapkan nomor bulan untuk garis kemajuan bulanan.
interval.MonthlyDayMonthNumber = 1;
// menetapkan nilai yang menunjukkan apakah menampilkan garis kemajuan berdasarkan hari pertama atau terakhir yang telah ditentukan.
interval.MonthlyFirstLast = true;
// menetapkan tipe hari pertama atau terakhir untuk garis kemajuan bulanan.
interval.MonthlyFirstLastDay = RecurringInterval.DayType.Day;
// menetapkan nomor bulan untuk garis kemajuan, yang ditampilkan berdasarkan hari pertama atau terakhir yang telah ditentukan.
interval.MonthlyFirstLastMonthNumber = 1;

view.ProgressLines.RecurringInterval = newInterval;

project.Save(OutDir + "WorkWithRecurringInterval_out.pdf", SaveFileFormat.Pdf);
```

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


