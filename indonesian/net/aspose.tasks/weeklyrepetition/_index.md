---
title: "Kelas WeeklyRepetition"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.WeeklyRepetition. Mewakili pola yang berbasis pada hari kerja"
type: docs
weight: 3590
url: /id/net/aspose.tasks/weeklyrepetition/
---
## WeeklyRepetition class

Mewakili pola yang berbasis pada hari kerja.

```csharp
public class WeeklyRepetition : WeeklyRepetitionBase
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [WeeklyRepetition](weeklyrepetition/)() | Menginisialisasi instance baru dari kelas `WeeklyRepetition`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | Mendapatkan atau mengatur jumlah minggu yang mewakili interval dalam minggu antara kejadian. |
| [WeekDays](../../aspose.tasks/weeklyrepetition/weekdays/) { get; set; } | Mendapatkan atau mengatur tipe hari kerja. |

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

* class [WeeklyRepetitionBase](../weeklyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


