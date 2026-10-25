---
title: "Enum WeekdayType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WeekdayType enum. Bir projenin RecurringTaskInfo sınıfı örneğinde bir hafta gününü temsil eder."
type: docs
weight: 3570
url: /tr/net/aspose.tasks/weekdaytype/
---
## WeekdayType enumeration

Bir projenin, [`RecurringTaskInfo`](../recurringtaskinfo/) sınıfı örneğinde bir hafta gününü temsil eder.

```csharp
[Flags]
public enum WeekdayType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | None hafta günü tipini gösterir. |
| Sunday | `1` | Pazar hafta günü tipini gösterir. |
| Monday | `2` | Pazartesi hafta günü tipini gösterir. |
| Tuesday | `4` | Salı hafta günü tipini gösterir. |
| Wednesday | `8` | Çarşamba hafta günü tipini gösterir. |
| Thursday | `10` | Perşembe hafta günü tipini gösterir. |
| Friday | `20` | Cuma hafta günü tipini gösterir. |
| Saturday | `40` | Cumartesi hafta günü tipini gösterir. |

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


