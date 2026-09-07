---
title: "ByYearDayRepetition.ByYearDayRepetition"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor ByYearDayRepetition. Menginisialisasi instance baru dari kelas ByYearDayRepetition"
type: docs
weight: 10
url: /id/net/aspose.tasks/byyeardayrepetition/byyeardayrepetition/
---
## ByYearDayRepetition constructor

Menginisialisasi instance baru dari kelas [`ByYearDayRepetition`](../).

```csharp
public ByYearDayRepetition()
```

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

* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


