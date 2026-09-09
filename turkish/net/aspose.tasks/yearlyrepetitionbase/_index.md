---
title: "Sınıf YearlyRepetitionBase"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.YearlyRepetitionBase sınıfı. Yıllık gün konumu için temel bir desen temsil eder."
type: docs
weight: 3700
url: /tr/net/aspose.tasks/yearlyrepetitionbase/
---
## YearlyRepetitionBase class

Yıllık gün konumu için temel bir deseni temsil eder.

```csharp
public abstract class YearlyRepetitionBase
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


