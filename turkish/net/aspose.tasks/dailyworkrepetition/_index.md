---
title: "Sınıf DailyWorkRepetition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.DailyWorkRepetition sınıfı. Çalışma günlerine dayalı günlük yineleme desenindeki tekrarları temsil eden bir sınıftır"
type: docs
weight: 420
url: /tr/net/aspose.tasks/dailyworkrepetition/
---
## DailyWorkRepetition class

Çalışma günlerine dayalı günlük yineleme desenindeki tekrarlar için bir sınıfı temsil eder.

```csharp
public class DailyWorkRepetition : DailyRepetitionBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [DailyWorkRepetition](dailyworkrepetition/)() | `DailyWorkRepetition` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | Oluşumlar arasındaki gün cinsinden aralığı temsil eden gün sayısını alır veya ayarlar. |

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

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


