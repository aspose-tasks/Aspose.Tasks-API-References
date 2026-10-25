---
title: "MonthlyRecurrencePattern.MonthlyRecurrencePattern"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor MonthlyRecurrencePattern. Menginisialisasi sebuah instance baru dari kelas MonthlyRecurrencePattern"
type: docs
weight: 10
url: /id/net/aspose.tasks/monthlyrecurrencepattern/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern constructor

Menginisialisasi sebuah instance baru dari kelas [`MonthlyRecurrencePattern`](../).

```csharp
public MonthlyRecurrencePattern()
```

## Contoh

Menampilkan cara bekerja dengan pengulangan pola berulang bulanan saat membuat tugas berulang.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [MonthlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../monthlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


