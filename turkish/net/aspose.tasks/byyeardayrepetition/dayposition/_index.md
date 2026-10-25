---
title: "ByYearDayRepetition.DayPosition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ByYearDayRepetition özelliği. Görevin tekrarlanması gereken ay içindeki gün konumunu alır veya ayarlar"
type: docs
weight: 20
url: /tr/net/aspose.tasks/byyeardayrepetition/dayposition/
---
## ByYearDayRepetition.DayPosition property

Görevin yinelenmesi gereken ay içindeki gün konumunu alır veya ayarlar.

```csharp
public int DayPosition { get; set; }
```

## Örnekler

Yeni yinelenen görevler oluştururken yıl günü tekrarlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


