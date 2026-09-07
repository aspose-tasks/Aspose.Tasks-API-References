---
title: "ByYearWeekDayRepetition.Position"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ByYearWeekDayRepetition. Mendapatkan atau mengatur posisi hari dalam minggu pada bulan di mana tugas harus berulang"
type: docs
weight: 30
url: /id/net/aspose.tasks/byyearweekdayrepetition/position/
---
## ByYearWeekDayRepetition.Position property

Mendapatkan atau mengatur posisi hari dalam minggu bulan di mana tugas harus berulang.

```csharp
public OrdinalNumber Position { get; set; }
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

* enum [OrdinalNumber](../../ordinalnumber/)
* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


