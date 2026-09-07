---
title: "Kelas RecurringTaskInfo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.RecurringTaskInfo. Mewakili detail dari tugas berulang dalam sebuah proyek"
type: docs
weight: 1720
url: /id/net/aspose.tasks/recurringtaskinfo/
---
## RecurringTaskInfo class

Mewakili detail tugas berulang dalam sebuah proyek.

```csharp
public class RecurringTaskInfo
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [DailyRepetitions](../../aspose.tasks/recurringtaskinfo/dailyrepetitions/) { get; set; } | Mendapatkan atau mengatur jumlah pengulangan untuk pola berulang harian. |
| [DailyUseWorkdays](../../aspose.tasks/recurringtaskinfo/dailyuseworkdays/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menggunakan hari kerja untuk pola berulang harian. |
| [Duration](../../aspose.tasks/recurringtaskinfo/duration/) { get; set; } | Mendapatkan atau mengatur durasi untuk satu kejadian tugas berulang. instance dari kelas [`Duration`](./duration/). |
| [EndDate](../../aspose.tasks/recurringtaskinfo/enddate/) { get; set; } | Mendapatkan atau mengatur tanggal berakhirnya kejadian. |
| [MonthlyDay](../../aspose.tasks/recurringtaskinfo/monthlyday/) { get; set; } | Mendapatkan atau mengatur jumlah hari pada pola berulang bulanan. |
| [MonthlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyordinalday/) { get; set; } | Mendapatkan atau mengatur hari pada pola berulang bulanan saat menggunakan hari ordinal. Bisa menjadi salah satu nilai dari enumerasi DayOfWeek. |
| [MonthlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/monthlyordinalnumber/) { get; set; } | Mendapatkan atau mengatur nomor ordinal pada pola berulang bulanan. Bisa menjadi salah satu nilai dari enumerasi [`OrdinalNumber`](../ordinalnumber/). |
| [MonthlyOrdinalRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyordinalrepetitions/) { get; set; } | Mendapatkan atau mengatur jumlah pengulangan untuk pola berulang bulanan saat menggunakan hari ordinal. |
| [MonthlyRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyrepetitions/) { get; set; } | Mendapatkan atau mengatur jumlah pengulangan untuk pola berulang bulanan. |
| [MonthlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyuseordinalday/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menggunakan hari ordinal untuk pola berulang bulanan. |
| [Occurrences](../../aspose.tasks/recurringtaskinfo/occurrences/) { get; set; } | Mendapatkan atau mengatur jumlah kejadian tugas berulang. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskinfo/recurrencepattern/) { get; set; } | Mendapatkan atau mengatur pola berulang tugas berulang. Bisa menjadi salah satu nilai dari enumerasi [`RecurrencePattern`](./recurrencepattern/). |
| [StartDate](../../aspose.tasks/recurringtaskinfo/startdate/) { get; set; } | Mendapatkan atau mengatur tanggal mulai kejadian. |
| [Task](../../aspose.tasks/recurringtaskinfo/task/) { get; } | Mendapatkan tugas induk dari instance kelas `RecurringTaskInfo` ini. |
| [UseEndDate](../../aspose.tasks/recurringtaskinfo/useenddate/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menggunakan tanggal akhir atau jumlah kejadian untuk tugas berulang. |
| [WeeklyDays](../../aspose.tasks/recurringtaskinfo/weeklydays/) { get; set; } | Mendapatkan atau mengatur koleksi hari yang digunakan dalam pola pengulangan mingguan. |
| [WeeklyRepetitions](../../aspose.tasks/recurringtaskinfo/weeklyrepetitions/) { get; set; } | Mendapatkan atau mengatur jumlah pengulangan untuk pola pengulangan mingguan. |
| [YearlyDate](../../aspose.tasks/recurringtaskinfo/yearlydate/) { get; set; } | Mendapatkan atau mengatur tanggal untuk pola pengulangan tahunan. |
| [YearlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyordinalday/) { get; set; } | Mendapatkan atau mengatur hari kerja dari pola pengulangan tahunan saat menggunakan hari ordinal. Bisa menjadi salah satu nilai dari enumerasi DayOfWeek. |
| [YearlyOrdinalMonth](../../aspose.tasks/recurringtaskinfo/yearlyordinalmonth/) { get; set; } | Mendapatkan atau mengatur bulan dari pola pengulangan tahunan saat menggunakan hari ordinal. Bisa menjadi salah satu nilai dari enumerasi [`Month`](../month/). |
| [YearlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/yearlyordinalnumber/) { get; set; } | Mendapatkan atau mengatur nomor ordinal dari pola pengulangan tahunan. Bisa menjadi salah satu nilai dari enumerasi [`OrdinalNumber`](../ordinalnumber/). |
| [YearlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyuseordinalday/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menggunakan hari ordinal untuk pola pengulangan tahunan. |

## Contoh

Menampilkan cara membaca informasi berulang dari tugas.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

// baca informasi berulang dari tugas
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    var info = task.RecurringInfo;
    if (info == null)
    {
        continue;
    }

    Console.WriteLine("Start Date: " + info.StartDate);
    Console.WriteLine("Duration: " + info.Duration);
    Console.WriteLine("End Date: " + info.EndDate);
    Console.WriteLine("Daily Repetitions: " + info.DailyRepetitions);
    Console.WriteLine("Daily Use Workdays: " + info.DailyUseWorkdays);
    Console.WriteLine("Monthly Day: " + info.MonthlyDay);
    Console.WriteLine("Monthly Ordinal Day: " + info.MonthlyOrdinalDay);
    Console.WriteLine("Monthly Ordinal Number: " + info.MonthlyOrdinalNumber);
    Console.WriteLine("Monthly Ordinal Repetitions: " + info.MonthlyOrdinalRepetitions);
    Console.WriteLine("Monthly Repetitions: " + info.MonthlyRepetitions);
    Console.WriteLine("Monthly Use Ordinal Day: " + info.MonthlyUseOrdinalDay);
    Console.WriteLine("Occurrences: " + info.Occurrences);
    Console.WriteLine("Recurrence Pattern: " + info.RecurrencePattern);
    Console.WriteLine("Parent Task: " + info.Task.Get(Tsk.Name));
    Console.WriteLine("Use End Date: " + info.UseEndDate);
    Console.WriteLine("Weekly Days: " + info.WeeklyDays);
    Console.WriteLine("Weekly Repetitions: " + info.WeeklyRepetitions);
    Console.WriteLine("Yearly Date: " + info.YearlyDate);
    Console.WriteLine("Yearly Ordinal Day: " + info.YearlyOrdinalDay);
    Console.WriteLine("Yearly Ordinal Month: " + info.YearlyOrdinalMonth);
    Console.WriteLine("Yearly Ordinal Number: " + info.YearlyOrdinalNumber);
    Console.WriteLine("Yearly Use Ordinal Day: " + info.YearlyUseOrdinalDay);
    Console.WriteLine();
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


