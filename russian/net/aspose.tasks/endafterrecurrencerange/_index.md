---
title: "Класс EndAfterRecurrenceRange"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.EndAfterRecurrenceRange. Представляет диапазон повторения повторяющейся задачи, ограниченный числом повторений"
type: docs
weight: 500
url: /ru/net/aspose.tasks/endafterrecurrencerange/
---
## EndAfterRecurrenceRange class

Представляет диапазон повторения повторяющейся задачи, ограниченный числом повторений.

```csharp
public class EndAfterRecurrenceRange : RecurrenceRangeBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [EndAfterRecurrenceRange](endafterrecurrencerange/)() | Инициализирует новый экземпляр класса `EndAfterRecurrenceRange`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [OccurrenceNumber](../../aspose.tasks/endafterrecurrencerange/occurrencenumber/) { get; set; } | Получает или задает количество повторений, ограничивающих диапазон повторения повторяющейся задачи. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Получает или задает дату начала диапазона повторения повторяющейся задачи. |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


