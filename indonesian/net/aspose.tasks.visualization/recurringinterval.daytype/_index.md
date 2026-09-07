---
title: "Enum RecurringInterval.DayType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.Visualization.RecurringIntervalDayType enum. Mewakili tipe hari yang digunakan dalam garis kemajuan"
type: docs
weight: 3320
url: /id/net/aspose.tasks.visualization/recurringinterval.daytype/
---
## RecurringInterval.DayType enumeration

Mewakili tipe hari yang digunakan dalam garis kemajuan.

```csharp
public enum DayType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Sunday | `1` | Menunjukkan Minggu. |
| Monday | `2` | Menunjukkan Senin. |
| Tuesday | `3` | Menunjukkan Selasa. |
| Wednesday | `4` | Menunjukkan Rabu. |
| Thursday | `5` | Menunjukkan Kamis. |
| Friday | `6` | Menunjukkan Jumat. |
| Saturday | `7` | Menunjukkan Sabtu. |
| Day | `8` | Menunjukkan Hari. |
| Workday | `9` | Menunjukkan hari kerja. |
| NonworkingDay | `10` | Menunjukkan hari non-kerja. |

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

* class [RecurringInterval](../recurringinterval/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


