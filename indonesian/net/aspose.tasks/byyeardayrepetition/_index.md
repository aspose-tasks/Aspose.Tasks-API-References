---
title: "Kelas ByYearDayRepetition"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ByYearDayRepetition. Mewakili pola yang didasarkan pada posisi absolut sebuah hari dalam sebulan."
type: docs
weight: 190
url: /id/net/aspose.tasks/byyeardayrepetition/
---
## ByYearDayRepetition class

Mewakili pola yang didasarkan pada posisi absolut suatu hari dalam sebulan.

```csharp
public class ByYearDayRepetition : YearlyRepetitionBase
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [ByYearDayRepetition](byyeardayrepetition/)() | Menginisialisasi instance baru dari kelas `ByYearDayRepetition`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [DayPosition](../../aspose.tasks/byyeardayrepetition/dayposition/) { get; set; } | Mendapatkan atau mengatur posisi hari dalam sebulan di mana tugas harus berulang. |
| [Month](../../aspose.tasks/byyeardayrepetition/month/) { get; set; } | Mendapatkan atau mengatur bulan di mana tugas harus berulang. |

## Contoh

Menampilkan cara bekerja dengan pengulangan hari tahunan saat membuat tugas berulang baru.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


