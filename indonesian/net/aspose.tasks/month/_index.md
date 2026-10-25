---
title: "Enum Month"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Month. Menentukan bulan."
type: docs
weight: 1040
url: /id/net/aspose.tasks/month/
---
## Month enumeration

Menentukan bulan.

```csharp
public enum Month
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Undefined | `-1` | Menunjukkan nilai tidak didefinisikan dalam file proyek asli. |
| January | `0` | Menunjukkan bulan Januari. |
| February | `1` | Menunjukkan bulan Februari. |
| March | `2` | Menunjukkan bulan Maret. |
| April | `3` | Menunjukkan bulan April. |
| May | `4` | Menunjukkan bulan Mei. |
| June | `5` | Menunjukkan bulan Juni. |
| July | `6` | Menunjukkan bulan Juli. |
| August | `7` | Menunjukkan bulan Agustus. |
| September | `8` | Menunjukkan bulan September. |
| October | `9` | Menunjukkan bulan Oktober. |
| November | `10` | Menunjukkan bulan November. |
| December | `11` | Menunjukkan bulan Desember. |

## Catatan

Saat mengekspor ke XML nilai Undefined akan dihilangkan dari XML yang dihasilkan.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


