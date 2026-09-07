---
title: "DailyRecurrencePattern.DailyRecurrencePattern"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor DailyRecurrencePattern. Menginisialisasi sebuah instance baru dari kelas DailyRecurrencePattern"
type: docs
weight: 10
url: /id/net/aspose.tasks/dailyrecurrencepattern/dailyrecurrencepattern/
---
## DailyRecurrencePattern constructor

Menginisialisasi sebuah instance baru dari kelas [`DailyRecurrencePattern`](../).

```csharp
public DailyRecurrencePattern()
```

## Contoh

Menampilkan cara bekerja dengan pengulangan pola kerja harian saat membuat tugas berulang.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "New recurrent task",
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     RecurrenceRange = new EndAfterRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 1, 1, 8, 0, 0), OccurrenceNumber = 9
                                                                           },
                                                     Repetition = new DailyWorkRepetition { RepetitionInterval = 1 }
                                                 },
                         Duration = project.GetDuration(1, TimeUnitType.Hour)
                     };
parameters.SetCalendar(project, "Standard");

var task = project.RootTask.Children.Add(parameters);
task.Set(Tsk.Start, new DateTime(2020, 4, 27, 8, 0, 0));

// lanjutkan bekerja dengan proyek...
// ...
```

### Lihat Juga

* class [DailyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../dailyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


