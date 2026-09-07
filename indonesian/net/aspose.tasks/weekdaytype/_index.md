---
title: "Enum WeekdayType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.WeekdayType enum. Mewakili hari kerja dari sebuah proyek dalam instance kelas RecurringTaskInfo."
type: docs
weight: 3570
url: /id/net/aspose.tasks/weekdaytype/
---
## WeekdayType enumeration

Mewakili hari kerja dari sebuah proyek dalam instance kelas [`RecurringTaskInfo`](../recurringtaskinfo/).

```csharp
[Flags]
public enum WeekdayType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| None | `0` | Menunjukkan tipe hari kerja None. |
| Sunday | `1` | Menunjukkan tipe hari kerja Sunday. |
| Monday | `2` | Menunjukkan tipe hari kerja Monday. |
| Tuesday | `4` | Menunjukkan tipe hari kerja Tuesday. |
| Wednesday | `8` | Menunjukkan tipe hari kerja Wednesday. |
| Thursday | `10` | Menunjukkan tipe hari kerja Thursday. |
| Friday | `20` | Menunjukkan tipe hari kerja Friday. |
| Saturday | `40` | Menunjukkan tipe hari kerja Saturday. |

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


