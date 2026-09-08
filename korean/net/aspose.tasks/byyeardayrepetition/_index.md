---
title: "클래스 ByYearDayRepetition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ByYearDayRepetition 클래스. 월 내 하루의 절대 위치를 기반으로 하는 패턴을 나타냅니다."
type: docs
weight: 190
url: /ko/net/aspose.tasks/byyeardayrepetition/
---
## ByYearDayRepetition class

월 내 일의 절대 위치를 기반으로 하는 패턴을 나타냅니다.

```csharp
public class ByYearDayRepetition : YearlyRepetitionBase
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ByYearDayRepetition](byyeardayrepetition/)() | `ByYearDayRepetition` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [DayPosition](../../aspose.tasks/byyeardayrepetition/dayposition/) { get; set; } | 작업이 반복되어야 하는 월 내 하루의 위치를 가져오거나 설정합니다. |
| [Month](../../aspose.tasks/byyeardayrepetition/month/) { get; set; } | 작업이 반복되어야 하는 월을 가져오거나 설정합니다. |

## 예제

새로운 반복 작업을 생성하면서 연도 일 반복을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


