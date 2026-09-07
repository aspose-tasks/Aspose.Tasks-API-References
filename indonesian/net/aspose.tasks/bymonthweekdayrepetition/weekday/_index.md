---
title: "ByMonthWeekDayRepetition.WeekDay"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ByMonthWeekDayRepetition. Mendapatkan atau mengatur tipe hari dalam minggu di mana tugas harus berulang"
type: docs
weight: 30
url: /id/net/aspose.tasks/bymonthweekdayrepetition/weekday/
---
## ByMonthWeekDayRepetition.WeekDay property

Mendapatkan atau mengatur tipe hari kerja di mana tugas harus berulang.

```csharp
public DayOfWeek WeekDay { get; set; }
```

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

* class [ByMonthWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


