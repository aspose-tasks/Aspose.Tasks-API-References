---
title: "ByMonthDayRepetition.DayPosition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ByMonthDayRepetition özelliği. Ay içinde görevin tekrarlanması gereken bir günün konumunu alır veya ayarlar"
type: docs
weight: 20
url: /tr/net/aspose.tasks/bymonthdayrepetition/dayposition/
---
## ByMonthDayRepetition.DayPosition property

Görevin tekrarlanması gereken ay içindeki gün konumunu alır veya ayarlar.

```csharp
public int DayPosition { get; set; }
```

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

* class [ByMonthDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthdayrepetition/)
* assembly [Aspose.Tasks](../../../)


