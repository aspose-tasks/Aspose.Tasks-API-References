---
title: "클래스 ByMonthDayRepetition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ByMonthDayRepetition 클래스. 월 내 하루의 절대 위치를 기반으로 하는 패턴을 나타냅니다."
type: docs
weight: 170
url: /ko/net/aspose.tasks/bymonthdayrepetition/
---
## ByMonthDayRepetition class

월 내 일의 절대 위치를 기반으로 하는 패턴을 나타냅니다.

```csharp
public class ByMonthDayRepetition : MonthlyRepetitionBase
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ByMonthDayRepetition](bymonthdayrepetition/)() | `ByMonthDayRepetition` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [DayPosition](../../aspose.tasks/bymonthdayrepetition/dayposition/) { get; set; } | 작업이 반복되어야 하는 월 내 하루의 위치를 가져오거나 설정합니다. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | 발생 간의 간격을 월 수로 나타내는 값을 가져오거나 설정합니다. |

## 예제

새 반복 작업을 만들면서 월 일 반복을 사용하는 방법을 보여줍니다.

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


