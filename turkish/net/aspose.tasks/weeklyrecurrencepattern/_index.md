---
title: "Sınıf WeeklyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WeeklyRecurrencePattern sınıfı. Bir projede haftalık yinelenen görev oluşturmak için kullanılan parametre kümesini temsil eder."
type: docs
weight: 3580
url: /tr/net/aspose.tasks/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern class

Projede haftalık yinelenen bir görev oluşturmak için kullanılan parametre kümesini temsil eder.

```csharp
public class WeeklyRecurrencePattern : RecurrencePatternBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WeeklyRecurrencePattern](weeklyrecurrencepattern/)() | Yeni bir `WeeklyRecurrencePattern` sınıfının örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Yineleme aralığını alır veya ayarlar. |
| [Repetition](../../aspose.tasks/weeklyrecurrencepattern/repetition/) { get; set; } | Tekrarlayan tekrar desenini alır veya ayarlar. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


