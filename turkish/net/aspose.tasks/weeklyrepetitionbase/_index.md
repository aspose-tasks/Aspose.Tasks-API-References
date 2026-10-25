---
title: "Sınıf WeeklyRepetitionBase"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WeeklyRepetitionBase sınıfı. Haftalık yineleme deseninde tekrarlar için temel bir sınıfı temsil eder."
type: docs
weight: 3600
url: /tr/net/aspose.tasks/weeklyrepetitionbase/
---
## WeeklyRepetitionBase class

Haftalık yinelenme desenindeki tekrarlar için temel bir sınıfı temsil eder.

```csharp
public abstract class WeeklyRepetitionBase
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | Tekrarlar arasındaki haftalık aralığı temsil eden hafta sayısını alır veya ayarlar. |

## Örnekler

Tekrarlayan bir görev nasıl oluşturulacağını gösterir.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "Recurring task",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new WeeklyRecurrencePattern
                                                 {
                                                     Repetition = new WeeklyRepetition
                                                                      {
                                                                          RepetitionInterval = 2,
                                                                          WeekDays = WeekdayType.Sunday | WeekdayType.Monday | WeekdayType.Friday
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 7, 20, 17, 0, 0)
                                                                           }
                                                 },
                         IgnoreResourceCalendar = false
                     };

parameters.SetCalendar(project, "Standard");

project.RootTask.Children.Add(parameters);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


