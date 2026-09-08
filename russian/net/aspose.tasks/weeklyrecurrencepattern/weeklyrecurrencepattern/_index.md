---
title: "WeeklyRecurrencePattern.WeeklyRecurrencePattern"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор WeeklyRecurrencePattern. Инициализирует новый экземпляр класса WeeklyRecurrencePattern"
type: docs
weight: 10
url: /ru/net/aspose.tasks/weeklyrecurrencepattern/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern constructor

Инициализирует новый экземпляр класса [`WeeklyRecurrencePattern`](../).

```csharp
public WeeklyRecurrencePattern()
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

* class [WeeklyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../weeklyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


