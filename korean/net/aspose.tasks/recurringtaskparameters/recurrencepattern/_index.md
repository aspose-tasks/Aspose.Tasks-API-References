---
title: "RecurringTaskParameters.RecurrencePattern"
second_title: "Aspose.Tasks for .NET API 참조"
description: "RecurringTaskParameters 속성. 반복 작업의 재발 패턴을 가져오거나 설정합니다. RecurrencePattern 열거형의 값 중 하나일 수 있습니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/recurringtaskparameters/recurrencepattern/
---
## RecurringTaskParameters.RecurrencePattern property

반복 작업의 재발 패턴을 가져오거나 설정합니다. `RecurrencePattern` 열거형의 값 중 하나일 수 있습니다.

```csharp
public RecurrencePatternBase RecurrencePattern { get; set; }
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

* class [RecurrencePatternBase](../../recurrencepatternbase/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


