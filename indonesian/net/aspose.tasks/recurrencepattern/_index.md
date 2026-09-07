---
title: "Enum RecurrencePattern"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.RecurrencePattern. Mewakili jenis pola berulang dari tugas berulang"
type: docs
weight: 1690
url: /id/net/aspose.tasks/recurrencepattern/
---
## RecurrencePattern enumeration

Mewakili jenis pola pengulangan dari tugas berulang.

```csharp
[Flags]
public enum RecurrencePattern
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Daily | `1` | Pola harian. |
| Weekly | `4` | Pola mingguan. |
| Monthly | `8` | Pola bulanan. |
| Yearly | `10` | Pola tahunan. |

## Contoh

Menampilkan cara membuat tugas berulang.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "Recurring task",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new WeeklyRecurrencePattern
                                                 {
                                                     Repetition = new WeeklyRepetition
                                                                      {
                                                                          RepetitionInterval = 2,
                                                                          WeekDays = WeekdayType.Sunday | WeekdayType.Monday | WeekdayType.Friday
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 7, 20, 17, 0, 0)
                                                                           }
                                                 },
                         IgnoreResourceCalendar = false
                     };

parameters.SetCalendar(project, "Standard");

project.RootTask.Children.Add(parameters);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


