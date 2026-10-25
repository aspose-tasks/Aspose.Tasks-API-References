---
title: "RecurringTaskParameters.IgnoreResourceCalendar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "RecurringTaskParameters özelliği. Kaynakların mevcut olmadığı zamanlarda bile yinelenen görevi planlayıp planlamayacağını belirten bir değeri alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/
---
## RecurringTaskParameters.IgnoreResourceCalendar property

Yinelenen görevi, kaynakların mevcut olup olmadığına bakılmaksızın planlayıp planlamayacağını gösteren bir değeri alır veya ayarlar.

```csharp
public bool IgnoreResourceCalendar { get; set; }
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

* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


