---
title: "RecurringTaskParameters.Duration"
second_title: "Aspose.Tasks for .NET API 참조"
description: "RecurringTaskParameters 속성. 반복 작업 한 번 발생에 대한 기간을 가져오거나 설정합니다. Duration 클래스의 인스턴스"
type: docs
weight: 20
url: /ko/net/aspose.tasks/recurringtaskparameters/duration/
---
## RecurringTaskParameters.Duration property

반복 작업 한 번 발생에 대한 기간을 가져오거나 설정합니다. `Duration` 클래스의 인스턴스.

```csharp
public Duration Duration { get; set; }
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

* struct [Duration](../../duration/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


