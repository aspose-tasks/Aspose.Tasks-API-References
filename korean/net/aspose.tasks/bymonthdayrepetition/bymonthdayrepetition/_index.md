---
title: "ByMonthDayRepetition.ByMonthDayRepetition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ByMonthDayRepetition 생성자. ByMonthDayRepetition 클래스의 새 인스턴스를 초기화합니다"
type: docs
weight: 10
url: /ko/net/aspose.tasks/bymonthdayrepetition/bymonthdayrepetition/
---
## ByMonthDayRepetition constructor

새 인스턴스를 초기화합니다 [`ByMonthDayRepetition`](../) 클래스의.

```csharp
public ByMonthDayRepetition()
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


