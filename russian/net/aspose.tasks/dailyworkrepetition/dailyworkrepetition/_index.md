---
title: "DailyWorkRepetition.DailyWorkRepetition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор DailyWorkRepetition. Инициализирует новый экземпляр класса DailyWorkRepetition"
type: docs
weight: 10
url: /ru/net/aspose.tasks/dailyworkrepetition/dailyworkrepetition/
---
## DailyWorkRepetition constructor

Инициализирует новый экземпляр класса [`DailyWorkRepetition`](../).

```csharp
public DailyWorkRepetition()
```

## Примеры

Показывает, как работать с повторениями шаблона ежедневного рабочего повторения при создании повторяющихся задач.

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

// работайте с проектом дальше...
// ...
```

### См. также

* class [DailyWorkRepetition](../)
* namespace [Aspose.Tasks](../../dailyworkrepetition/)
* assembly [Aspose.Tasks](../../../)


