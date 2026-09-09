---
title: "WeeklyRepetition sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WeeklyRepetition sınıfı. Haftanın günlerine dayalı bir desen temsil eder"
type: docs
weight: 3590
url: /tr/net/aspose.tasks/weeklyrepetition/
---
## WeeklyRepetition class

Hafta günlerine dayalı bir deseni temsil eder.

```csharp
public class WeeklyRepetition : WeeklyRepetitionBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WeeklyRepetition](weeklyrepetition/)() | `WeeklyRepetition` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | Tekrarlar arasındaki haftalık aralığı temsil eden hafta sayısını alır veya ayarlar. |
| [WeekDays](../../aspose.tasks/weeklyrepetition/weekdays/) { get; set; } | Haftanın günleri türünü alır veya ayarlar. |

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

* class [WeeklyRepetitionBase](../weeklyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


