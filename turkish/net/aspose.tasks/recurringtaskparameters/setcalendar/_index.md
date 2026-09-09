---
title: "RecurringTaskParameters.SetCalendar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "RecurringTaskParameters yöntemi. Yinelenen görev için bir takvim ayarlar. Takvim, proje takvim koleksiyonundan seçilir"
type: docs
weight: 60
url: /tr/net/aspose.tasks/recurringtaskparameters/setcalendar/
---
## RecurringTaskParameters.SetCalendar method

Yinelenen görev için bir takvim ayarlayın. Takvim, proje takvim koleksiyonundan seçilir.

```csharp
public void SetCalendar(Project project, string calendarName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| project | Project | Takvim koleksiyonuna sahip proje. |
| calendarName | Dize | Takvimin adı. |

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

* class [Project](../../project/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


