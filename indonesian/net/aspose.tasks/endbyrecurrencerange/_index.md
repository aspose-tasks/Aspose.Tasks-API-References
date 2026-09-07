---
title: "Kelas EndByRecurrenceRange"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.EndByRecurrenceRange. Mewakili rentang pengulangan tugas berulang yang dibatasi oleh hari selesai"
type: docs
weight: 510
url: /id/net/aspose.tasks/endbyrecurrencerange/
---
## EndByRecurrenceRange class

Mewakili rentang pengulangan tugas berulang yang dibatasi oleh hari selesai.

```csharp
public class EndByRecurrenceRange : RecurrenceRangeBase
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [EndByRecurrenceRange](endbyrecurrencerange/)() | Menginisialisasi instance baru dari kelas `EndByRecurrenceRange`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Finish](../../aspose.tasks/endbyrecurrencerange/finish/) { get; set; } | Mendapatkan atau mengatur tanggal yang membatasi rentang pengulangan tugas berulang. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Mendapatkan atau mengatur tanggal mulai rentang pengulangan tugas berulang. |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


