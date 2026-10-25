---
title: "Sınıf DailyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.DailyRecurrencePattern sınıfı. Bir projede günlük yinelenen bir görev oluşturmak için kullanılan parametre kümesini temsil eder."
type: docs
weight: 400
url: /tr/net/aspose.tasks/dailyrecurrencepattern/
---
## DailyRecurrencePattern class

Bir projede günlük yinelenen bir görev oluşturmak için kullanılan parametre kümesini temsil eder.

```csharp
public class DailyRecurrencePattern : RecurrencePatternBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [DailyRecurrencePattern](dailyrecurrencepattern/)() | `DailyRecurrencePattern` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Yineleme aralığını alır veya ayarlar. |
| [Repetition](../../aspose.tasks/dailyrecurrencepattern/repetition/) { get; set; } | Günlük yineleme desenindeki tekrar desenini alır veya ayarlar. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


