---
title: "Kelas ByYearWeekDayRepetition"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ByYearWeekDayRepetition. Mewakili pola yang berdasarkan pada posisi hari kerja dalam sebulan."
type: docs
weight: 200
url: /id/net/aspose.tasks/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition class

Mewakili pola yang didasarkan pada posisi hari kerja dalam sebulan.

```csharp
public class ByYearWeekDayRepetition : YearlyRepetitionBase
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [ByYearWeekDayRepetition](byyearweekdayrepetition/)() | Menginisialisasi sebuah instance baru dari kelas `ByYearWeekDayRepetition`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Month](../../aspose.tasks/byyearweekdayrepetition/month/) { get; set; } | Mendapatkan atau mengatur bulan di mana tugas harus berulang. |
| [Position](../../aspose.tasks/byyearweekdayrepetition/position/) { get; set; } | Mendapatkan atau mengatur posisi hari dalam minggu bulan di mana tugas harus berulang. |
| [WeekDay](../../aspose.tasks/byyearweekdayrepetition/weekday/) { get; set; } | Mendapatkan atau mengatur tipe hari dalam seminggu di mana tugas harus berulang. |

## Contoh

Menampilkan cara bekerja dengan pengulangan hari dalam tahun saat membuat tugas berulang baru.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearWeekDayRepetition
                                                                      {
                                                                          Month = Month.July, WeekDay = DayOfWeek.Sunday, Position = OrdinalNumber.First
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 31, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearWeekDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


