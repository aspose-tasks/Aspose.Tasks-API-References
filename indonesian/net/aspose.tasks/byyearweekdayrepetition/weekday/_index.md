---
title: "ByYearWeekDayRepetition.WeekDay"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ByYearWeekDayRepetition. Mendapatkan atau mengatur tipe hari dalam minggu di mana tugas harus berulang"
type: docs
weight: 40
url: /id/net/aspose.tasks/byyearweekdayrepetition/weekday/
---
## ByYearWeekDayRepetition.WeekDay property

Mendapatkan atau mengatur tipe hari dalam seminggu di mana tugas harus berulang.

```csharp
public DayOfWeek WeekDay { get; set; }
```

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

* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


