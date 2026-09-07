---
title: "Kelas ByMonthWeekDayRepetition"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ByMonthWeekDayRepetition. Mewakili pola yang berdasarkan pada posisi hari kerja dalam sebulan"
type: docs
weight: 180
url: /id/net/aspose.tasks/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition class

Mewakili pola yang didasarkan pada posisi hari kerja dalam sebulan.

```csharp
public class ByMonthWeekDayRepetition : MonthlyRepetitionBase
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [ByMonthWeekDayRepetition](bymonthweekdayrepetition/)() | Menginisialisasi sebuah instance baru dari kelas `ByMonthWeekDayRepetition`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Position](../../aspose.tasks/bymonthweekdayrepetition/position/) { get; set; } | Mendapatkan atau mengatur posisi hari kerja dalam sebulan di mana tugas harus berulang. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Mendapatkan atau mengatur jumlah bulan yang mewakili interval dalam bulan antara kejadian. |
| [WeekDay](../../aspose.tasks/bymonthweekdayrepetition/weekday/) { get; set; } | Mendapatkan atau mengatur tipe hari kerja di mana tugas harus berulang. |

## Contoh

Menampilkan cara bekerja dengan pengulangan hari kerja bulanan saat membuat tugas berulang baru.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthWeekDayRepetition
                                                                      {
                                                                          Position = OrdinalNumber.First,
                                                                          WeekDay = DayOfWeek.Sunday,
                                                                          RepetitionInterval = 2
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 2, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);
project.Save(OutDir + "CanAddRecurringTask_Months_WeekDay_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


