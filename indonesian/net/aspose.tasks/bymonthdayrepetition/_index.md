---
title: "Class ByMonthDayRepetition"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ByMonthDayRepetition. Mewakili pola yang berdasarkan pada posisi absolut hari dalam sebulan."
type: docs
weight: 170
url: /id/net/aspose.tasks/bymonthdayrepetition/
---
## ByMonthDayRepetition class

Mewakili pola yang didasarkan pada posisi absolut suatu hari dalam sebulan.

```csharp
public class ByMonthDayRepetition : MonthlyRepetitionBase
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [ByMonthDayRepetition](bymonthdayrepetition/)() | Menginisialisasi instance baru dari kelas `ByMonthDayRepetition`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [DayPosition](../../aspose.tasks/bymonthdayrepetition/dayposition/) { get; set; } | Mendapatkan atau mengatur posisi hari dalam sebulan dimana tugas harus berulang. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Mendapatkan atau mengatur jumlah bulan yang mewakili interval dalam bulan antara kejadian. |

## Contoh

Menampilkan cara bekerja dengan pengulangan hari bulan saat membuat tugas berulang baru.

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


