---
title: "Перечисление WeekdayType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.WeekdayType. Представляет день недели проекта в экземпляре класса RecurringTaskInfo."
type: docs
weight: 3570
url: /ru/net/aspose.tasks/weekdaytype/
---
## WeekdayType enumeration

Представляет день недели проекта в экземпляре класса [`RecurringTaskInfo`](../recurringtaskinfo/).

```csharp
[Flags]
public enum WeekdayType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Указывает тип дня недели None. |
| Sunday | `1` | Указывает тип дня недели Sunday. |
| Monday | `2` | Указывает тип дня недели Monday. |
| Tuesday | `4` | Указывает тип дня недели Tuesday. |
| Wednesday | `8` | Указывает тип дня недели Wednesday. |
| Thursday | `10` | Указывает тип дня недели Thursday. |
| Friday | `20` | Указывает тип дня недели Friday. |
| Saturday | `40` | Указывает тип дня недели Saturday. |

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


