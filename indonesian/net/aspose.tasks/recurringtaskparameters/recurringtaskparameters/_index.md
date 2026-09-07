---
title: "RecurringTaskParameters.RecurringTaskParameters"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor RecurringTaskParameters. Menginisialisasi instance baru dari kelas RecurringTaskParameters."
type: docs
weight: 10
url: /id/net/aspose.tasks/recurringtaskparameters/recurringtaskparameters/
---
## RecurringTaskParameters constructor

Menginisialisasi instance baru dari kelas [`RecurringTaskParameters`](../).

```csharp
public RecurringTaskParameters()
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

* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


