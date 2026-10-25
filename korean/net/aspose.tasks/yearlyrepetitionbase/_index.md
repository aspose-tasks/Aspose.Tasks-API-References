---
title: "클래스 YearlyRepetitionBase"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.YearlyRepetitionBase 클래스. 연간 일 위치에 대한 기본 패턴을 나타냅니다."
type: docs
weight: 3700
url: /ko/net/aspose.tasks/yearlyrepetitionbase/
---
## YearlyRepetitionBase class

연간 일 위치를 위한 기본 패턴을 나타냅니다.

```csharp
public abstract class YearlyRepetitionBase
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


