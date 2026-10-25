---
title: "DailyRepetitionBase.RepetitionInterval"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "DailyRepetitionBase özelliği. Oluşumlar arasındaki gün cinsinden aralığı temsil eden gün sayısını alır veya ayarlar."
type: docs
weight: 10
url: /tr/net/aspose.tasks/dailyrepetitionbase/repetitioninterval/
---
## DailyRepetitionBase.RepetitionInterval property

Oluşumlar arasındaki gün cinsinden aralığı temsil eden gün sayısını alır veya ayarlar.

```csharp
public int RepetitionInterval { get; set; }
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

* class [DailyRepetitionBase](../)
* namespace [Aspose.Tasks](../../dailyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


