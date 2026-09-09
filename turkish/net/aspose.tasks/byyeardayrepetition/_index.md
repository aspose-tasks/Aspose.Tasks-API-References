---
title: "Sınıf ByYearDayRepetition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ByYearDayRepetition sınıfı. Bir ay içindeki günün mutlak konumuna dayalı bir deseni temsil eder."
type: docs
weight: 190
url: /tr/net/aspose.tasks/byyeardayrepetition/
---
## ByYearDayRepetition class

Ay içinde bir günün mutlak konumuna dayalı bir deseni temsil eder.

```csharp
public class ByYearDayRepetition : YearlyRepetitionBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ByYearDayRepetition](byyeardayrepetition/)() | `ByYearDayRepetition` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DayPosition](../../aspose.tasks/byyeardayrepetition/dayposition/) { get; set; } | Görevin yinelenmesi gereken ay içindeki gün konumunu alır veya ayarlar. |
| [Month](../../aspose.tasks/byyeardayrepetition/month/) { get; set; } | Görevin yinelenmesi gereken ayı alır veya ayarlar. |

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

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


