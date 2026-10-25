---
title: "Kelas WeeklyRecurrencePattern"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.WeeklyRecurrencePattern. Mewakili sekumpulan parameter yang digunakan untuk membuat tugas berulang mingguan dalam sebuah proyek"
type: docs
weight: 3580
url: /id/net/aspose.tasks/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern class

Mewakili kumpulan parameter yang digunakan untuk membuat tugas berulang mingguan dalam sebuah proyek.

```csharp
public class WeeklyRecurrencePattern : RecurrencePatternBase
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [WeeklyRecurrencePattern](weeklyrecurrencepattern/)() | Menginisialisasi instance baru dari kelas `WeeklyRecurrencePattern`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Mendapatkan atau mengatur rentang pengulangan. |
| [Repetition](../../aspose.tasks/weeklyrecurrencepattern/repetition/) { get; set; } | Mendapatkan atau mengatur pola pengulangan berulang. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


