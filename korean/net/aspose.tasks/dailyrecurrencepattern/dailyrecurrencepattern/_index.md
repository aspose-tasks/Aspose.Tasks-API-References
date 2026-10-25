---
title: "DailyRecurrencePattern.DailyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API 참조"
description: "DailyRecurrencePattern 생성자. DailyRecurrencePattern 클래스의 새 인스턴스를 초기화합니다"
type: docs
weight: 10
url: /ko/net/aspose.tasks/dailyrecurrencepattern/dailyrecurrencepattern/
---
## DailyRecurrencePattern constructor

[`DailyRecurrencePattern`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public DailyRecurrencePattern()
```

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

* class [DailyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../dailyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


