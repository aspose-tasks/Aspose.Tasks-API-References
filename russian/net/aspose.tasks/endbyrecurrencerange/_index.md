---
title: "Класс EndByRecurrenceRange"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.EndByRecurrenceRange. Представляет диапазон повторения повторяющейся задачи, ограниченный датой завершения."
type: docs
weight: 510
url: /ru/net/aspose.tasks/endbyrecurrencerange/
---
## EndByRecurrenceRange class

Представляет диапазон повторения повторяющейся задачи, ограниченный датой завершения.

```csharp
public class EndByRecurrenceRange : RecurrenceRangeBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [EndByRecurrenceRange](endbyrecurrencerange/)() | Инициализирует новый экземпляр класса `EndByRecurrenceRange`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Finish](../../aspose.tasks/endbyrecurrencerange/finish/) { get; set; } | Получает или задает дату, ограничивающую диапазон повторения повторяющейся задачи. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Получает или задает дату начала диапазона повторения повторяющейся задачи. |

## Примеры

Показывает, как создать повторяющуюся задачу.

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

### См. также

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


