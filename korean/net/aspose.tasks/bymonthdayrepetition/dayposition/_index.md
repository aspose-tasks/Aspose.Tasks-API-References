---
title: "ByMonthDayRepetition.DayPosition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ByMonthDayRepetition 속성. 작업이 반복되어야 하는 월 내 일자의 위치를 가져오거나 설정합니다"
type: docs
weight: 20
url: /ko/net/aspose.tasks/bymonthdayrepetition/dayposition/
---
## ByMonthDayRepetition.DayPosition property

작업이 반복되어야 하는 월 내 하루의 위치를 가져오거나 설정합니다.

```csharp
public int DayPosition { get; set; }
```

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

* class [ByMonthDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthdayrepetition/)
* assembly [Aspose.Tasks](../../../)


