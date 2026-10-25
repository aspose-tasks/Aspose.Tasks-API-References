---
title: "Enum RecurrencePattern"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.RecurrencePattern enum. Tekrarlayan bir görevin yineleme deseninin türünü temsil eder."
type: docs
weight: 1690
url: /tr/net/aspose.tasks/recurrencepattern/
---
## RecurrencePattern enumeration

Tekrarlayan bir görevin yineleme deseninin bir türünü temsil eder.

```csharp
[Flags]
public enum RecurrencePattern
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Daily | `1` | Günlük desen. |
| Weekly | `4` | Haftalık desen. |
| Monthly | `8` | Aylık desen. |
| Yearly | `10` | Yıllık desen. |

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


