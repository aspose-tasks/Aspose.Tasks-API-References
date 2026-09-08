---
title: "EndAfterRecurrenceRange.EndAfterRecurrenceRange"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор EndAfterRecurrenceRange. Инициализирует новый экземпляр класса EndAfterRecurrenceRange"
type: docs
weight: 10
url: /ru/net/aspose.tasks/endafterrecurrencerange/endafterrecurrencerange/
---
## EndAfterRecurrenceRange constructor

Инициализирует новый экземпляр класса [`EndAfterRecurrenceRange`](../).

```csharp
public EndAfterRecurrenceRange()
```

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

* class [EndAfterRecurrenceRange](../)
* namespace [Aspose.Tasks](../../endafterrecurrencerange/)
* assembly [Aspose.Tasks](../../../)


