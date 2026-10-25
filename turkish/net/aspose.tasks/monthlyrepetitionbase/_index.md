---
title: "Sınıf MonthlyRepetitionBase"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.MonthlyRepetitionBase sınıfı. Aylık gün konumu için temel bir deseni temsil eder."
type: docs
weight: 1090
url: /tr/net/aspose.tasks/monthlyrepetitionbase/
---
## MonthlyRepetitionBase class

Aylık gün konumu için temel bir deseni temsil eder.

```csharp
public abstract class MonthlyRepetitionBase
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Tekrarlar arasındaki ay aralığını temsil eden ay sayısını alır veya ayarlar. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


