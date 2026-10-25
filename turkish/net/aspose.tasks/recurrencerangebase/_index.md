---
title: "Sınıf RecurrenceRangeBase"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.RecurrenceRangeBase sınıfı. Yinelenen bir görevin yineleme aralığını temsil eder."
type: docs
weight: 1710
url: /tr/net/aspose.tasks/recurrencerangebase/
---
## RecurrenceRangeBase class

Yineleyen görevin yineleme aralığını temsil eder.

```csharp
public abstract class RecurrenceRangeBase
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Tekrarlayan görevin tekrarlama aralığının başlangıç tarihini alır veya ayarlar. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


