---
title: "WeeklyRecurrencePattern.Repetition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "WeeklyRecurrencePattern 속성. 반복 패턴을 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/weeklyrecurrencepattern/repetition/
---
## WeeklyRecurrencePattern.Repetition property

반복되는 반복 패턴을 가져오거나 설정합니다.

```csharp
public WeeklyRepetitionBase Repetition { get; set; }
```

## 예제

반복 작업을 만드는 방법을 보여줍니다.

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

### 또 보기

* class [WeeklyRepetitionBase](../../weeklyrepetitionbase/)
* class [WeeklyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../weeklyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


