---
title: "Kelas RecurringTaskParameters"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.RecurringTaskParameters. Mewakili sekumpulan parameter yang digunakan untuk membuat tugas berulang dalam sebuah proyek."
type: docs
weight: 1730
url: /id/net/aspose.tasks/recurringtaskparameters/
---
## RecurringTaskParameters class

Mewakili sekumpulan parameter yang digunakan untuk membuat tugas berulang dalam sebuah proyek.

```csharp
public class RecurringTaskParameters
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [RecurringTaskParameters](recurringtaskparameters/)() | Menginisialisasi instance baru dari kelas `RecurringTaskParameters`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Duration](../../aspose.tasks/recurringtaskparameters/duration/) { get; set; } | Mendapatkan atau mengatur durasi untuk satu kejadian tugas berulang. Instance dari kelas [`Duration`](./duration/). |
| [IgnoreResourceCalendar](../../aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menjadwalkan tugas berulang meskipun tidak terjadi ketika tidak ada sumber daya yang tersedia untuk mengerjakannya. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskparameters/recurrencepattern/) { get; set; } | Mendapatkan atau mengatur pola pengulangan tugas berulang. Dapat berupa salah satu nilai dari enumerasi [`RecurrencePattern`](./recurrencepattern/). |
| [TaskName](../../aspose.tasks/recurringtaskparameters/taskname/) { get; set; } | Mendapatkan atau mengatur nama tugas berulang. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [SetCalendar](../../aspose.tasks/recurringtaskparameters/setcalendar/)(Project, string) | Atur kalender untuk tugas berulang. Kalender dipilih dari koleksi kalender proyek. |

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


