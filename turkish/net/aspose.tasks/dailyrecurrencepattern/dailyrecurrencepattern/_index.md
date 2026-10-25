---
title: "DailyRecurrencePattern.DailyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "DailyRecurrencePattern yapıcı. DailyRecurrencePattern sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks/dailyrecurrencepattern/dailyrecurrencepattern/
---
## DailyRecurrencePattern constructor

[`DailyRecurrencePattern`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public DailyRecurrencePattern()
```

## Örnekler

Yinelenen görevler oluştururken günlük iş tekrar desenindeki tekrarlarla nasıl çalışılacağını gösterir.

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

// projeyle daha fazla çalış...
// ...
```

### Ayrıca Bakınız

* class [DailyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../dailyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


