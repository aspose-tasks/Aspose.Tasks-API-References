---
title: "클래스 DailyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.DailyRecurrencePattern 클래스. 프로젝트에서 매일 반복 작업을 생성하는 데 사용되는 매개변수 집합을 나타냅니다"
type: docs
weight: 400
url: /ko/net/aspose.tasks/dailyrecurrencepattern/
---
## DailyRecurrencePattern class

프로젝트에서 일일 반복 작업을 생성하는 데 사용되는 매개변수 집합을 나타냅니다.

```csharp
public class DailyRecurrencePattern : RecurrencePatternBase
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [DailyRecurrencePattern](dailyrecurrencepattern/)() | `DailyRecurrencePattern` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | 반복 범위를 가져오거나 설정합니다. |
| [Repetition](../../aspose.tasks/dailyrecurrencepattern/repetition/) { get; set; } | 일일 반복 패턴에서 반복 패턴을 가져오거나 설정합니다. |

## 예제

반복 작업을 생성하는 동안 일일 작업 반복 패턴 반복을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "New recurrent task",
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     RecurrenceRange = new EndAfterRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 1, 1, 8, 0, 0), OccurrenceNumber = 9
                                                                           },
                                                     Repetition = new DailyWorkRepetition { RepetitionInterval = 1 }
                                                 },
                         Duration = project.GetDuration(1, TimeUnitType.Hour)
                     };
parameters.SetCalendar(project, "Standard");

var task = project.RootTask.Children.Add(parameters);
task.Set(Tsk.Start, new DateTime(2020, 4, 27, 8, 0, 0));

// 프로젝트를 계속 작업합니다...
// ...
```

### 또 보기

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


