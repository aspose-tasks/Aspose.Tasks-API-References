---
title: "Class ByMonthDayRepetition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ByMonthDayRepetition sınıfı. Bir ay içindeki günün mutlak konumuna dayalı bir deseni temsil eder."
type: docs
weight: 170
url: /tr/net/aspose.tasks/bymonthdayrepetition/
---
## ByMonthDayRepetition class

Ay içinde bir günün mutlak konumuna dayalı bir deseni temsil eder.

```csharp
public class ByMonthDayRepetition : MonthlyRepetitionBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ByMonthDayRepetition](bymonthdayrepetition/)() | `ByMonthDayRepetition` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DayPosition](../../aspose.tasks/bymonthdayrepetition/dayposition/) { get; set; } | Görevin tekrarlanması gereken ay içindeki gün konumunu alır veya ayarlar. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Tekrarlar arasındaki ay aralığını temsil eden ay sayısını alır veya ayarlar. |

## Örnekler

Yeni bir tekrarlayan görev oluştururken ay gün tekrarlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


