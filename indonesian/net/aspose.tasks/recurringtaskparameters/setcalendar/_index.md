---
title: "RecurringTaskParameters.SetCalendar"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode RecurringTaskParameters. Menetapkan kalender untuk tugas berulang. Kalender dipilih dari koleksi kalender proyek."
type: docs
weight: 60
url: /id/net/aspose.tasks/recurringtaskparameters/setcalendar/
---
## RecurringTaskParameters.SetCalendar method

Atur kalender untuk tugas berulang. Kalender dipilih dari koleksi kalender proyek.

```csharp
public void SetCalendar(Project project, string calendarName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| proyek | Project | Proyek dengan koleksi kalender. |
| calendarName | String | Nama kalender. |

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

* class [Project](../../project/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


