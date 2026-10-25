---
title: "Класс DailyRepetitionBase"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.DailyRepetitionBase класс. Представляет базовый класс для повторений в ежедневном шаблоне повторения"
type: docs
weight: 410
url: /ru/net/aspose.tasks/dailyrepetitionbase/
---
## DailyRepetitionBase class

Представляет базовый класс для повторений в ежедневном шаблоне повторения.

```csharp
public abstract class DailyRepetitionBase
```

## Свойства

| Имя | Описание |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | Получает или задает количество дней, которое представляет интервал в днях между вхождениями. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


