---
title: "Sınıf YearlyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.YearlyRecurrencePattern sınıfı. Bir projede yıllık yinelenen görev oluşturmak için kullanılan parametre kümesini temsil eder"
type: docs
weight: 3690
url: /tr/net/aspose.tasks/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern class

Projede yıllık yinelenen bir görev oluşturmak için kullanılan parametre kümesini temsil eder.

```csharp
public class YearlyRecurrencePattern : RecurrencePatternBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [YearlyRecurrencePattern](yearlyrecurrencepattern/)() | `YearlyRecurrencePattern` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Yineleme aralığını alır veya ayarlar. |
| [Repetition](../../aspose.tasks/yearlyrecurrencepattern/repetition/) { get; set; } | Yinelenen konum desenini alır veya ayarlar. |

## Örnekler

Yinelenen görevler oluştururken yıl yıl yinelenen desenlerle nasıl çalışılacağını gösterir.

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

project.Save(OutDir + "WorkWithYearlyRecurrencePattern_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


