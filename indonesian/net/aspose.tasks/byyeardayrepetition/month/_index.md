---
title: "ByYearDayRepetition.Month"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ByYearDayRepetition. Mendapatkan atau mengatur bulan di mana tugas harus berulang"
type: docs
weight: 30
url: /id/net/aspose.tasks/byyeardayrepetition/month/
---
## ByYearDayRepetition.Month property

Mendapatkan atau mengatur bulan di mana tugas harus berulang.

```csharp
public Month Month { get; set; }
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

* enum [Month](../../month/)
* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


