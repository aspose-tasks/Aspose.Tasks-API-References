---
title: "RecurringTaskParameters.RecurrencePattern"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство RecurringTaskParameters. Получает или задает шаблон повторения повторяющейся задачи. Может быть одним из значений перечисления RecurrencePattern."
type: docs
weight: 40
url: /ru/net/aspose.tasks/recurringtaskparameters/recurrencepattern/
---
## RecurringTaskParameters.RecurrencePattern property

Получает или задает шаблон повторения повторяющейся задачи. Может быть одним из значений перечисления `RecurrencePattern`.

```csharp
public RecurrencePatternBase RecurrencePattern { get; set; }
```

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

* class [RecurrencePatternBase](../../recurrencepatternbase/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


