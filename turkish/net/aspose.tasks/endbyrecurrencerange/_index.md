---
title: "Sınıf EndByRecurrenceRange"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.EndByRecurrenceRange sınıfı. Bitirme gününe göre sınırlı olan yinelenen görevin tekrarlama aralığını temsil eder"
type: docs
weight: 510
url: /tr/net/aspose.tasks/endbyrecurrencerange/
---
## EndByRecurrenceRange class

Bitiş günü ile sınırlı yinelenen görevin yineleme aralığını temsil eder.

```csharp
public class EndByRecurrenceRange : RecurrenceRangeBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [EndByRecurrenceRange](endbyrecurrencerange/)() | Yeni bir `EndByRecurrenceRange` sınıfı örneği başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Finish](../../aspose.tasks/endbyrecurrencerange/finish/) { get; set; } | Yinelenen görevin tekrarlama aralığını sınırlayan tarihi alır veya ayarlar. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Tekrarlayan görevin tekrarlama aralığının başlangıç tarihini alır veya ayarlar. |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


