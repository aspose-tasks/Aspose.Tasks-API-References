---
title: "Класс WeeklyRecurrencePattern"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.WeeklyRecurrencePattern. Представляет набор параметров, используемых для создания еженедельной повторяющейся задачи в проекте."
type: docs
weight: 3580
url: /ru/net/aspose.tasks/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern class

Представляет набор параметров, используемых для создания еженедельной повторяющейся задачи в проекте.

```csharp
public class WeeklyRecurrencePattern : RecurrencePatternBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WeeklyRecurrencePattern](weeklyrecurrencepattern/)() | Инициализирует новый экземпляр класса `WeeklyRecurrencePattern`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Получает или задает диапазон повторения. |
| [Repetition](../../aspose.tasks/weeklyrecurrencepattern/repetition/) { get; set; } | Получает или задает повторяющийся шаблон. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


