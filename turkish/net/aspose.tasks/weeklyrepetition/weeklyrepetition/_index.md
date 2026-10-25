---
title: "WeeklyRepetition.WeeklyRepetition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "WeeklyRepetition yapıcı. WeeklyRepetition sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks/weeklyrepetition/weeklyrepetition/
---
## WeeklyRepetition constructor

Yeni bir [`WeeklyRepetition`](../) sınıfının örneğini başlatır.

```csharp
public WeeklyRepetition()
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

* class [WeeklyRepetition](../)
* namespace [Aspose.Tasks](../../weeklyrepetition/)
* assembly [Aspose.Tasks](../../../)


