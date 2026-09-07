---
title: "RecurringTaskInfo.MonthlyOrdinalDay"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti RecurringTaskInfo. Mendapatkan atau mengatur hari dalam pola pengulangan bulanan ketika menggunakan hari ordinal. Bisa menjadi salah satu nilai dari enumerasi DayOfWeek."
type: docs
weight: 60
url: /id/net/aspose.tasks/recurringtaskinfo/monthlyordinalday/
---
## RecurringTaskInfo.MonthlyOrdinalDay property

Mendapatkan atau mengatur hari pada pola berulang bulanan saat menggunakan hari ordinal. Bisa menjadi salah satu nilai dari enumerasi DayOfWeek.

```csharp
public DayOfWeek MonthlyOrdinalDay { get; set; }
```

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

* class [RecurringTaskInfo](../)
* namespace [Aspose.Tasks](../../recurringtaskinfo/)
* assembly [Aspose.Tasks](../../../)


