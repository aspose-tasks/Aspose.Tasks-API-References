---
title: "클래스 WeeklyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WeeklyRecurrencePattern 클래스. 프로젝트에서 주간 반복 작업을 생성하는 데 사용되는 매개변수 집합을 나타냅니다."
type: docs
weight: 3580
url: /ko/net/aspose.tasks/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern class

프로젝트에서 주간 반복 작업을 만들 때 사용되는 매개변수 집합을 나타냅니다.

```csharp
public class WeeklyRecurrencePattern : RecurrencePatternBase
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [WeeklyRecurrencePattern](weeklyrecurrencepattern/)() | `WeeklyRecurrencePattern` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | 반복 범위를 가져오거나 설정합니다. |
| [Repetition](../../aspose.tasks/weeklyrecurrencepattern/repetition/) { get; set; } | 반복되는 반복 패턴을 가져오거나 설정합니다. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


