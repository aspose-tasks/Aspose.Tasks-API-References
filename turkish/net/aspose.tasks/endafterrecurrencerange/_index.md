---
title: "Sınıf EndAfterRecurrenceRange"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.EndAfterRecurrenceRange sınıfı. Tekrar eden görevin, oluşum sayısı ile sınırlı tekrarlama aralığını temsil eder."
type: docs
weight: 500
url: /tr/net/aspose.tasks/endafterrecurrencerange/
---
## EndAfterRecurrenceRange class

Oluşum sayısı ile sınırlı yinelenen görevin yineleme aralığını temsil eder.

```csharp
public class EndAfterRecurrenceRange : RecurrenceRangeBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [EndAfterRecurrenceRange](endafterrecurrencerange/)() | `EndAfterRecurrenceRange` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [OccurrenceNumber](../../aspose.tasks/endafterrecurrencerange/occurrencenumber/) { get; set; } | Tekrarlayan görevin tekrarlama aralığını sınırlayan oluşum sayısını alır veya ayarlar. |
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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


