---
title: "클래스 EndByRecurrenceRange"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.EndByRecurrenceRange 클래스. 완료일에 의해 제한되는 반복 작업의 반복 범위를 나타냅니다."
type: docs
weight: 510
url: /ko/net/aspose.tasks/endbyrecurrencerange/
---
## EndByRecurrenceRange class

완료 일자로 제한되는 반복 작업의 반복 범위를 나타냅니다.

```csharp
public class EndByRecurrenceRange : RecurrenceRangeBase
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [EndByRecurrenceRange](endbyrecurrencerange/)() | `EndByRecurrenceRange` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Finish](../../aspose.tasks/endbyrecurrencerange/finish/) { get; set; } | 반복 작업의 반복 범위를 제한하는 날짜를 가져오거나 설정합니다. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | 반복 작업의 반복 범위 시작 날짜를 가져오거나 설정합니다. |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


