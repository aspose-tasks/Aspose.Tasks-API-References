---
title: "Класс DailyRecurrencePattern"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.DailyRecurrencePattern класс. Представляет набор параметров, используемых для создания ежедневной повторяющейся задачи в проекте"
type: docs
weight: 400
url: /ru/net/aspose.tasks/dailyrecurrencepattern/
---
## DailyRecurrencePattern class

Представляет набор параметров, используемых для создания ежедневной повторяющейся задачи в проекте.

```csharp
public class DailyRecurrencePattern : RecurrencePatternBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [DailyRecurrencePattern](dailyrecurrencepattern/)() | Инициализирует новый экземпляр класса `DailyRecurrencePattern`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Получает или задает диапазон повторения. |
| [Repetition](../../aspose.tasks/dailyrecurrencepattern/repetition/) { get; set; } | Получает или задает шаблон повторений в ежедневном шаблоне повторения. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


