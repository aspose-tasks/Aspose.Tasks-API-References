---
title: "Kelas MonthlyRecurrencePattern"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.MonthlyRecurrencePattern. Mewakili sekumpulan parameter yang digunakan untuk membuat tugas berulang bulanan dalam sebuah proyek."
type: docs
weight: 1080
url: /id/net/aspose.tasks/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern class

Mewakili sekumpulan parameter yang digunakan untuk membuat tugas berulang bulanan dalam sebuah proyek.

```csharp
public class MonthlyRecurrencePattern : RecurrencePatternBase
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [MonthlyRecurrencePattern](monthlyrecurrencepattern/)() | Menginisialisasi sebuah instance baru dari kelas `MonthlyRecurrencePattern`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Mendapatkan atau mengatur rentang pengulangan. |
| [Repetition](../../aspose.tasks/monthlyrecurrencepattern/repetition/) { get; set; } | Mendapatkan atau mengatur pola pengulangan berulang. |

## Contoh

Menampilkan cara bekerja dengan pengulangan pola berulang bulanan saat membuat tugas berulang.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


