---
title: "ByYearWeekDayRepetition.Position"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ByYearWeekDayRepetition özelliği. Görevin tekrarlanması gereken ayın bir haftasındaki gün konumunu alır veya ayarlar."
type: docs
weight: 30
url: /tr/net/aspose.tasks/byyearweekdayrepetition/position/
---
## ByYearWeekDayRepetition.Position property

Görevin yinelenmesi gereken ayın haftasındaki gün konumunu alır veya ayarlar.

```csharp
public OrdinalNumber Position { get; set; }
```

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

* enum [OrdinalNumber](../../ordinalnumber/)
* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


