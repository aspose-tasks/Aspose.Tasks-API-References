---
title: "Enum Interval"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Visualization.Interval. Menentukan interval berulang untuk menampilkan garis kemajuan pada"
type: docs
weight: 3170
url: /id/net/aspose.tasks.visualization/interval/
---
## Interval enumeration

Menentukan interval berulang untuk menampilkan garis kemajuan pada.

```csharp
public enum Interval
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Daily | `0` | Menunjukkan interval Harian. |
| Weekly | `1` | Menunjukkan interval Mingguan. |
| Monthly | `2` | Menunjukkan interval Bulanan. |

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


