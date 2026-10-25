---
title: "ByYearWeekDayRepetition sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ByYearWeekDayRepetition sınıfı. Bir ay içinde haftanın gününün konumuna dayalı bir deseni temsil eder."
type: docs
weight: 200
url: /tr/net/aspose.tasks/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition class

Ay içinde bir haftanın gününün konumuna dayalı bir deseni temsil eder.

```csharp
public class ByYearWeekDayRepetition : YearlyRepetitionBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ByYearWeekDayRepetition](byyearweekdayrepetition/)() | `ByYearWeekDayRepetition` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Month](../../aspose.tasks/byyearweekdayrepetition/month/) { get; set; } | Görevin yinelenmesi gereken ayı alır veya ayarlar. |
| [Position](../../aspose.tasks/byyearweekdayrepetition/position/) { get; set; } | Görevin yinelenmesi gereken ayın haftasındaki gün konumunu alır veya ayarlar. |
| [WeekDay](../../aspose.tasks/byyearweekdayrepetition/weekday/) { get; set; } | Görevin yinelenmesi gereken haftanın gün türünü alır veya ayarlar. |

## Örnekler

Yeni yinelenen görevler oluştururken yıl içindeki hafta günü tekrarlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearWeekDayRepetition
                                                                      {
                                                                          Month = Month.July, WeekDay = DayOfWeek.Sunday, Position = OrdinalNumber.First
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 31, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearWeekDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


