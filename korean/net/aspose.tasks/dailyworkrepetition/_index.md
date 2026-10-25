---
title: "클래스 DailyWorkRepetition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.DailyWorkRepetition 클래스. 작업일을 기준으로 하는 일일 반복 패턴의 반복을 나타내는 클래스입니다."
type: docs
weight: 420
url: /ko/net/aspose.tasks/dailyworkrepetition/
---
## DailyWorkRepetition class

근무일을 기반으로 하는 일일 반복 패턴의 반복을 위한 클래스를 나타냅니다.

```csharp
public class DailyWorkRepetition : DailyRepetitionBase
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [DailyWorkRepetition](dailyworkrepetition/)() | `DailyWorkRepetition` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | 발생 간의 일 수 간격을 나타내는 일 수를 가져오거나 설정합니다. |

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

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


