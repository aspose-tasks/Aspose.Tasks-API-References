---
title: "Sınıf MonthlyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.MonthlyRecurrencePattern sınıfı. Bir projede aylık yinelenen görev oluşturmak için kullanılan parametre kümesini temsil eder."
type: docs
weight: 1080
url: /tr/net/aspose.tasks/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern class

Bir projede aylık yinelenen görev oluşturmak için kullanılan parametre kümesini temsil eder.

```csharp
public class MonthlyRecurrencePattern : RecurrencePatternBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [MonthlyRecurrencePattern](monthlyrecurrencepattern/)() | `MonthlyRecurrencePattern` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Yineleme aralığını alır veya ayarlar. |
| [Repetition](../../aspose.tasks/monthlyrecurrencepattern/repetition/) { get; set; } | Tekrarlayan tekrar desenini alır veya ayarlar. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


