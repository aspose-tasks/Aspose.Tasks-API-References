---
title: "ByYearDayRepetition.Month"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ByYearDayRepetition 속성. 작업이 반복되어야 하는 월을 가져오거나 설정합니다"
type: docs
weight: 30
url: /ko/net/aspose.tasks/byyeardayrepetition/month/
---
## ByYearDayRepetition.Month property

작업이 반복되어야 하는 월을 가져오거나 설정합니다.

```csharp
public Month Month { get; set; }
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

* enum [Month](../../month/)
* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


