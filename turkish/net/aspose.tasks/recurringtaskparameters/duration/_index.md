---
title: "RecurringTaskParameters.Duration"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "RecurringTaskParameters özelliği. Yinelenen görevin bir oluşumu için süresi alır veya ayarlar. Duration sınıfının örneği"
type: docs
weight: 20
url: /tr/net/aspose.tasks/recurringtaskparameters/duration/
---
## RecurringTaskParameters.Duration property

Yinelenen görevin bir oluşumu için süresi alır veya ayarlar. `Duration` sınıfının örneği.

```csharp
public Duration Duration { get; set; }
```

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

* struct [Duration](../../duration/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


