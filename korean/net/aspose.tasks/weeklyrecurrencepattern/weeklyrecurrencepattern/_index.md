---
title: "WeeklyRecurrencePattern.WeeklyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API 참조"
description: "WeeklyRecurrencePattern 생성자. WeeklyRecurrencePattern 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/weeklyrecurrencepattern/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern constructor

[`WeeklyRecurrencePattern`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public WeeklyRecurrencePattern()
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

* class [WeeklyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../weeklyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


