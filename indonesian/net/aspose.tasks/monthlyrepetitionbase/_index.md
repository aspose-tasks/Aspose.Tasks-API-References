---
title: "Kelas MonthlyRepetitionBase"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.MonthlyRepetitionBase. Mewakili pola dasar untuk posisi hari bulanan"
type: docs
weight: 1090
url: /id/net/aspose.tasks/monthlyrepetitionbase/
---
## MonthlyRepetitionBase class

Mewakili pola dasar untuk posisi hari bulanan.

```csharp
public abstract class MonthlyRepetitionBase
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Mendapatkan atau mengatur jumlah bulan yang mewakili interval dalam bulan antara kejadian. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


