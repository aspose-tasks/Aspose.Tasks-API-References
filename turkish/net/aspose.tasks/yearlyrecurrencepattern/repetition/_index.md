---
title: "YearlyRecurrencePattern.Repetition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "YearlyRecurrencePattern özelliği. Tekrarlayan konum desenini alır veya ayarlar"
type: docs
weight: 20
url: /tr/net/aspose.tasks/yearlyrecurrencepattern/repetition/
---
## YearlyRecurrencePattern.Repetition property

Yinelenen konum desenini alır veya ayarlar.

```csharp
public YearlyRepetitionBase Repetition { get; set; }
```

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

* class [YearlyRepetitionBase](../../yearlyrepetitionbase/)
* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


