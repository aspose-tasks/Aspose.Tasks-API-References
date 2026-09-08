---
title: "클래스 MonthlyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.MonthlyRecurrencePattern 클래스. 프로젝트에서 월별 반복 작업을 생성하는 데 사용되는 매개변수 집합을 나타냅니다."
type: docs
weight: 1080
url: /ko/net/aspose.tasks/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern class

프로젝트에서 월간 반복 작업을 만들 때 사용되는 매개변수 집합을 나타냅니다.

```csharp
public class MonthlyRecurrencePattern : RecurrencePatternBase
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [MonthlyRecurrencePattern](monthlyrecurrencepattern/)() | `MonthlyRecurrencePattern` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | 반복 범위를 가져오거나 설정합니다. |
| [Repetition](../../aspose.tasks/monthlyrecurrencepattern/repetition/) { get; set; } | 반복되는 반복 패턴을 가져오거나 설정합니다. |

## 예제

반복 작업을 생성하면서 월별 반복 패턴 반복을 다루는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


