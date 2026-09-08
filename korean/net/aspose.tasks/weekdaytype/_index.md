---
title: "열거형 WeekdayType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WeekdayType enum. 프로젝트의 RecurringTaskInfo 클래스 인스턴스에서 요일을 나타냅니다"
type: docs
weight: 3570
url: /ko/net/aspose.tasks/weekdaytype/
---
## WeekdayType enumeration

프로젝트의 [`RecurringTaskInfo`](../recurringtaskinfo/) 클래스 인스턴스에서 요일을 나타냅니다.

```csharp
[Flags]
public enum WeekdayType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| None | `0` | None 요일 유형을 나타냅니다. |
| Sunday | `1` | Sunday 요일 유형을 나타냅니다. |
| Monday | `2` | Monday 요일 유형을 나타냅니다. |
| Tuesday | `4` | Tuesday 요일 유형을 나타냅니다. |
| Wednesday | `8` | Wednesday 요일 유형을 나타냅니다. |
| Thursday | `10` | Thursday 요일 유형을 나타냅니다. |
| Friday | `20` | Friday 요일 유형을 나타냅니다. |
| Saturday | `40` | Saturday 요일 유형을 나타냅니다. |

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


