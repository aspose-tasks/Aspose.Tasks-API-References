---
title: "MonthlyRepetitionBase.RepetitionInterval"
second_title: "Aspose.Tasks for .NET API 참조"
description: "MonthlyRepetitionBase 속성. 발생 간의 간격을 월 단위로 나타내는 개월 수를 가져오거나 설정합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/monthlyrepetitionbase/repetitioninterval/
---
## MonthlyRepetitionBase.RepetitionInterval property

발생 간의 간격을 월 수로 나타내는 값을 가져오거나 설정합니다.

```csharp
public int RepetitionInterval { get; set; }
```

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

* class [MonthlyRepetitionBase](../)
* namespace [Aspose.Tasks](../../monthlyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


