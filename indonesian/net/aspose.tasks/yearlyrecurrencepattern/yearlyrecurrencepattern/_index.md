---
title: "YearlyRecurrencePattern.YearlyRecurrencePattern"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor YearlyRecurrencePattern. Menginisialisasi instance baru dari kelas YearlyRecurrencePattern"
type: docs
weight: 10
url: /id/net/aspose.tasks/yearlyrecurrencepattern/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern constructor

Menginisialisasi instance baru dari kelas [`YearlyRecurrencePattern`](../).

```csharp
public YearlyRecurrencePattern()
```

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

* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


