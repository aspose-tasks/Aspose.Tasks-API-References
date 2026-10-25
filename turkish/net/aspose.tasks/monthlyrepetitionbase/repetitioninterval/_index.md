---
title: "MonthlyRepetitionBase.RepetitionInterval"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "MonthlyRepetitionBase özelliği. Oluşumlar arasındaki ay cinsinden aralığı temsil eden ay sayısını alır veya ayarlar."
type: docs
weight: 10
url: /tr/net/aspose.tasks/monthlyrepetitionbase/repetitioninterval/
---
## MonthlyRepetitionBase.RepetitionInterval property

Tekrarlar arasındaki ay aralığını temsil eden ay sayısını alır veya ayarlar.

```csharp
public int RepetitionInterval { get; set; }
```

## Örnekler

Tekrarlayan görevler oluştururken aylık yinelenme deseni tekrarlarıyla nasıl çalışılacağını gösterir.

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

* class [MonthlyRepetitionBase](../)
* namespace [Aspose.Tasks](../../monthlyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


