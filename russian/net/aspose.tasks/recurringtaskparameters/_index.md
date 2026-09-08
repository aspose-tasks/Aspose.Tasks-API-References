---
title: "Класс RecurringTaskParameters"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.RecurringTaskParameters. Представляет набор параметров, используемых для создания повторяющейся задачи в проекте"
type: docs
weight: 1730
url: /ru/net/aspose.tasks/recurringtaskparameters/
---
## RecurringTaskParameters class

Представляет набор параметров, используемых для создания повторяющейся задачи в проекте.

```csharp
public class RecurringTaskParameters
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [RecurringTaskParameters](recurringtaskparameters/)() | Инициализирует новый экземпляр класса `RecurringTaskParameters`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Duration](../../aspose.tasks/recurringtaskparameters/duration/) { get; set; } | Получает или задаёт продолжительность одного появления повторяющейся задачи. Экземпляр класса [`Duration`](./duration/). |
| [IgnoreResourceCalendar](../../aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/) { get; set; } | Получает или задаёт значение, указывающее, следует ли планировать повторяющуюся задачу, даже если она не может быть выполнена, когда нет доступных ресурсов. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskparameters/recurrencepattern/) { get; set; } | Получает или задаёт шаблон повторения повторяющейся задачи. Может быть одним из значений перечисления [`RecurrencePattern`](./recurrencepattern/). |
| [TaskName](../../aspose.tasks/recurringtaskparameters/taskname/) { get; set; } | Получает или задаёт имя повторяющейся задачи. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetCalendar](../../aspose.tasks/recurringtaskparameters/setcalendar/)(Project, string) | Установите календарь для повторяющейся задачи. Календарь выбирается из коллекции календарей проекта. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


