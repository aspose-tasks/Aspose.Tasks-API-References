---
title: "RecurringInterval.MonthlyDayMonthNumber"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti RecurringInterval. Mendapatkan atau mengatur nomor bulan dari garis kemajuan bulanan"
type: docs
weight: 70
url: /id/net/aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/
---
## RecurringInterval.MonthlyDayMonthNumber property

Mendapatkan atau mengatur nomor bulan dari garis kemajuan bulanan.

```csharp
public int MonthlyDayMonthNumber { get; set; }
```

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

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


