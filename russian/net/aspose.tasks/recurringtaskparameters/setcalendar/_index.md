---
title: "RecurringTaskParameters.SetCalendar"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод RecurringTaskParameters. Устанавливает календарь для повторяющейся задачи. Календарь выбирается из коллекции календарей проекта."
type: docs
weight: 60
url: /ru/net/aspose.tasks/recurringtaskparameters/setcalendar/
---
## RecurringTaskParameters.SetCalendar method

Установите календарь для повторяющейся задачи. Календарь выбирается из коллекции календарей проекта.

```csharp
public void SetCalendar(Project project, string calendarName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| проект | Project | Проект с коллекцией календарей. |
| calendarName | Строка | Имя календаря. |

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

* class [Project](../../project/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


