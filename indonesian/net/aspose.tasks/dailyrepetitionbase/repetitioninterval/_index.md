---
title: "DailyRepetitionBase.RepetitionInterval"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "DailyRepetitionBase property. Mendapatkan atau mengatur jumlah hari yang mewakili interval dalam hari antara kejadian"
type: docs
weight: 10
url: /id/net/aspose.tasks/dailyrepetitionbase/repetitioninterval/
---
## DailyRepetitionBase.RepetitionInterval property

Mendapatkan atau mengatur jumlah hari yang mewakili interval dalam hari antara kejadian.

```csharp
public int RepetitionInterval { get; set; }
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

* class [DailyRepetitionBase](../)
* namespace [Aspose.Tasks](../../dailyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


