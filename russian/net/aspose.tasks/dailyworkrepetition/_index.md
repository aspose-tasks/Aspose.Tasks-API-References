---
title: "Класс DailyWorkRepetition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.DailyWorkRepetition. Представляет класс для повторений в ежедневном шаблоне повторения, основанном на рабочих днях"
type: docs
weight: 420
url: /ru/net/aspose.tasks/dailyworkrepetition/
---
## DailyWorkRepetition class

Представляет класс для повторений в ежедневном шаблоне повторения, основанном на рабочих днях.

```csharp
public class DailyWorkRepetition : DailyRepetitionBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [DailyWorkRepetition](dailyworkrepetition/)() | Инициализирует новый экземпляр класса `DailyWorkRepetition`. |

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

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


