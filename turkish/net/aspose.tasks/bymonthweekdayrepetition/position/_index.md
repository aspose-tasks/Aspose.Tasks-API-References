---
title: "ByMonthWeekDayRepetition.Position"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ByMonthWeekDayRepetition özelliği. Görevin tekrarlanması gereken ay içinde haftanın gününün konumunu alır veya ayarlar"
type: docs
weight: 20
url: /tr/net/aspose.tasks/bymonthweekdayrepetition/position/
---
## ByMonthWeekDayRepetition.Position property

Görevin tekrarlanması gereken ay içinde haftanın gününün konumunu alır veya ayarlar.

```csharp
public OrdinalNumber Position { get; set; }
```

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

* enum [OrdinalNumber](../../ordinalnumber/)
* class [ByMonthWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


