---
title: "YearlyRecurrencePattern 클래스"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.YearlyRecurrencePattern 클래스. 프로젝트에서 연간 반복 작업을 만들 때 사용되는 매개변수 집합을 나타냅니다."
type: docs
weight: 3690
url: /ko/net/aspose.tasks/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern class

프로젝트에서 연간 반복 작업을 만들 때 사용되는 매개변수 집합을 나타냅니다.

```csharp
public class YearlyRecurrencePattern : RecurrencePatternBase
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [YearlyRecurrencePattern](yearlyrecurrencepattern/)() | 새 `YearlyRecurrencePattern` 클래스 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | 반복 범위를 가져오거나 설정합니다. |
| [Repetition](../../aspose.tasks/yearlyrecurrencepattern/repetition/) { get; set; } | 반복 위치 패턴을 가져오거나 설정합니다. |

## 예제

연도 연도 반복 패턴을 사용하면서 반복 작업을 만드는 방법을 보여줍니다.

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

project.Save(OutDir + "WorkWithYearlyRecurrencePattern_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


