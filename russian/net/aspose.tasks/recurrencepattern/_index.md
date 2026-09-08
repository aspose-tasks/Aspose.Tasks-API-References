---
title: "Перечисление RecurrencePattern"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.RecurrencePattern. Представляет тип шаблона повторения повторяющейся задачи."
type: docs
weight: 1690
url: /ru/net/aspose.tasks/recurrencepattern/
---
## RecurrencePattern enumeration

Представляет тип шаблона повторения повторяющейся задачи.

```csharp
[Flags]
public enum RecurrencePattern
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Daily | `1` | Ежедневный шаблон. |
| Weekly | `4` | Еженедельный шаблон. |
| Monthly | `8` | Ежемесячный шаблон. |
| Yearly | `10` | Ежегодный шаблон. |

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


