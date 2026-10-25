---
title: "열거형 RecurrencePattern"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.RecurrencePattern 열거형. 반복 작업의 재발 패턴 유형을 나타냅니다."
type: docs
weight: 1690
url: /ko/net/aspose.tasks/recurrencepattern/
---
## RecurrencePattern enumeration

반복 작업의 재발 패턴 유형을 나타냅니다.

```csharp
[Flags]
public enum RecurrencePattern
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Daily | `1` | 일일 패턴. |
| Weekly | `4` | 주간 패턴. |
| Monthly | `8` | 월간 패턴. |
| Yearly | `10` | 연간 패턴. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


