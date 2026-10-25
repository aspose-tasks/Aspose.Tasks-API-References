---
title: "WeeklyRepetition 클래스"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WeeklyRepetition 클래스. 평일을 기반으로 하는 패턴을 나타냅니다."
type: docs
weight: 3590
url: /ko/net/aspose.tasks/weeklyrepetition/
---
## WeeklyRepetition class

요일을 기반으로 하는 패턴을 나타냅니다.

```csharp
public class WeeklyRepetition : WeeklyRepetitionBase
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [WeeklyRepetition](weeklyrepetition/)() | `WeeklyRepetition` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | 발생 간의 간격을 주 단위로 나타내는 주 수를 가져오거나 설정합니다. |
| [WeekDays](../../aspose.tasks/weeklyrepetition/weekdays/) { get; set; } | 평일 유형을 가져오거나 설정합니다. |

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

* class [WeeklyRepetitionBase](../weeklyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


