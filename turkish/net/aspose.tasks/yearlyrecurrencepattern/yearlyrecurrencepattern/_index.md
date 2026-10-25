---
title: "YearlyRecurrencePattern.YearlyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "YearlyRecurrencePattern yapıcı. YearlyRecurrencePattern sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks/yearlyrecurrencepattern/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern constructor

[`YearlyRecurrencePattern`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public YearlyRecurrencePattern()
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

* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


