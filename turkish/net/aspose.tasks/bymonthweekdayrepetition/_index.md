---
title: "ByMonthWeekDayRepetition Sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ByMonthWeekDayRepetition sınıfı. Bir ay içinde haftanın gününün konumuna dayalı bir deseni temsil eder."
type: docs
weight: 180
url: /tr/net/aspose.tasks/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition class

Ay içinde haftanın gününün konumuna dayalı bir deseni temsil eder.

```csharp
public class ByMonthWeekDayRepetition : MonthlyRepetitionBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ByMonthWeekDayRepetition](bymonthweekdayrepetition/)() | `ByMonthWeekDayRepetition` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Position](../../aspose.tasks/bymonthweekdayrepetition/position/) { get; set; } | Görevin tekrarlanması gereken ay içinde haftanın gününün konumunu alır veya ayarlar. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Tekrarlar arasındaki ay aralığını temsil eden ay sayısını alır veya ayarlar. |
| [WeekDay](../../aspose.tasks/bymonthweekdayrepetition/weekday/) { get; set; } | Görevin tekrarlanması gereken haftanın gününün tipini alır veya ayarlar. |

## Örnekler

Yeni bir yinelenen görev oluştururken ay haftası tekrarlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthWeekDayRepetition
                                                                      {
                                                                          Position = OrdinalNumber.First,
                                                                          WeekDay = DayOfWeek.Sunday,
                                                                          RepetitionInterval = 2
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 2, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);
project.Save(OutDir + "CanAddRecurringTask_Months_WeekDay_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


