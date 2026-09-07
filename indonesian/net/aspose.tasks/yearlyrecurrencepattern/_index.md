---
title: "Kelas YearlyRecurrencePattern"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.YearlyRecurrencePattern. Mewakili sekumpulan parameter yang digunakan untuk membuat tugas berulang tahunan dalam sebuah proyek"
type: docs
weight: 3690
url: /id/net/aspose.tasks/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern class

Mewakili kumpulan parameter yang digunakan untuk membuat tugas berulang tahunan dalam sebuah proyek.

```csharp
public class YearlyRecurrencePattern : RecurrencePatternBase
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [YearlyRecurrencePattern](yearlyrecurrencepattern/)() | Menginisialisasi instance baru dari kelas `YearlyRecurrencePattern`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Mendapatkan atau mengatur rentang pengulangan. |
| [Repetition](../../aspose.tasks/yearlyrecurrencepattern/repetition/) { get; set; } | Mendapatkan atau mengatur pola posisi berulang. |

## Contoh

Menunjukkan cara bekerja dengan pola berulang tahunan saat membuat tugas berulang.

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

project.Save(OutDir + "WorkWithYearlyRecurrencePattern_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


