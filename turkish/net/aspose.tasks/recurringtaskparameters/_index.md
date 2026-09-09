---
title: "Sınıf RecurringTaskParameters"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.RecurringTaskParameters sınıfı. Bir projede yinelenen görev oluşturmak için kullanılan parametre kümesini temsil eder"
type: docs
weight: 1730
url: /tr/net/aspose.tasks/recurringtaskparameters/
---
## RecurringTaskParameters class

Bir projede yineleyen bir görev oluşturmak için kullanılan parametre setini temsil eder.

```csharp
public class RecurringTaskParameters
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [RecurringTaskParameters](recurringtaskparameters/)() | `RecurringTaskParameters` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Duration](../../aspose.tasks/recurringtaskparameters/duration/) { get; set; } | Yinelenen görevin bir oluşumu için süreyi alır veya ayarlar. [`Duration`](./duration/) sınıfının örneği. |
| [IgnoreResourceCalendar](../../aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/) { get; set; } | Yinelenen görevi, kaynakların mevcut olup olmadığına bakılmaksızın planlayıp planlamayacağını gösteren bir değeri alır veya ayarlar. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskparameters/recurrencepattern/) { get; set; } | Yinelenen görevin tekrarlama desenini alır veya ayarlar. [`RecurrencePattern`](./recurrencepattern/) enum değerlerinden biri olabilir. |
| [TaskName](../../aspose.tasks/recurringtaskparameters/taskname/) { get; set; } | Yinelenen görevin adını alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetCalendar](../../aspose.tasks/recurringtaskparameters/setcalendar/)(Project, string) | Yinelenen görev için bir takvim ayarlayın. Takvim, proje takvim koleksiyonundan seçilir. |

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


