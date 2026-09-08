---
title: "Класс WeeklyRepetition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.WeeklyRepetition. Представляет шаблон, основанный на будних днях"
type: docs
weight: 3590
url: /ru/net/aspose.tasks/weeklyrepetition/
---
## WeeklyRepetition class

Представляет шаблон, основанный на днях недели.

```csharp
public class WeeklyRepetition : WeeklyRepetitionBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WeeklyRepetition](weeklyrepetition/)() | Инициализирует новый экземпляр класса `WeeklyRepetition`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | Получает или задает количество недель, представляющее интервал в неделях между появлениями. |
| [WeekDays](../../aspose.tasks/weeklyrepetition/weekdays/) { get; set; } | Получает или задает тип будних дней. |

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

* class [WeeklyRepetitionBase](../weeklyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


