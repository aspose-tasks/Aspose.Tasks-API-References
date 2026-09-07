---
title: "WeeklyRepetition.WeekDays"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti WeeklyRepetition. Mendapatkan atau mengatur tipe hari kerja"
type: docs
weight: 20
url: /id/net/aspose.tasks/weeklyrepetition/weekdays/
---
## WeeklyRepetition.WeekDays property

Mendapatkan atau mengatur tipe hari kerja.

```csharp
public WeekdayType WeekDays { get; set; }
```

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

* enum [WeekdayType](../../weekdaytype/)
* class [WeeklyRepetition](../)
* namespace [Aspose.Tasks](../../weeklyrepetition/)
* assembly [Aspose.Tasks](../../../)


