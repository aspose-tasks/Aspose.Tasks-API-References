---
title: "RecurrencePatternBase.RecurrenceRange"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство RecurrencePatternBase. Получает или задаёт диапазон повторения"
type: docs
weight: 10
url: /ru/net/aspose.tasks/recurrencepatternbase/recurrencerange/
---
## RecurrencePatternBase.RecurrenceRange property

Получает или задает диапазон повторения.

```csharp
public RecurrenceRangeBase RecurrenceRange { get; set; }
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

* class [RecurrenceRangeBase](../../recurrencerangebase/)
* class [RecurrencePatternBase](../)
* namespace [Aspose.Tasks](../../recurrencepatternbase/)
* assembly [Aspose.Tasks](../../../)


