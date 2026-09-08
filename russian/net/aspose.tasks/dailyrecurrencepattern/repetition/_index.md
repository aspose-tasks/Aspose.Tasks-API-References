---
title: "DailyRecurrencePattern.Repetition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство DailyRecurrencePattern. Возвращает или задает шаблон повторений в ежедневном шаблоне повторения"
type: docs
weight: 20
url: /ru/net/aspose.tasks/dailyrecurrencepattern/repetition/
---
## DailyRecurrencePattern.Repetition property

Получает или задает шаблон повторений в ежедневном шаблоне повторения.

```csharp
public DailyRepetitionBase Repetition { get; set; }
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

* class [DailyRepetitionBase](../../dailyrepetitionbase/)
* class [DailyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../dailyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


