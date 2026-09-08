---
title: "RecurrenceRangeBase.Start"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство RecurrenceRangeBase. Получает или задаёт дату начала диапазона повторения повторяющейся задачи."
type: docs
weight: 10
url: /ru/net/aspose.tasks/recurrencerangebase/start/
---
## RecurrenceRangeBase.Start property

Получает или задает дату начала диапазона повторения повторяющейся задачи.

```csharp
public DateTime Start { get; set; }
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

* class [RecurrenceRangeBase](../)
* namespace [Aspose.Tasks](../../recurrencerangebase/)
* assembly [Aspose.Tasks](../../../)


