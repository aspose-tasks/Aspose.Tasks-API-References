---
title: "ByMonthWeekDayRepetition.WeekDay"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ByMonthWeekDayRepetition 속성. 작업이 반복되어야 하는 요일 유형을 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/bymonthweekdayrepetition/weekday/
---
## ByMonthWeekDayRepetition.WeekDay property

작업이 반복되어야 하는 요일 유형을 가져오거나 설정합니다.

```csharp
public DayOfWeek WeekDay { get; set; }
```

## 예제

새 반복 작업을 생성하면서 월 요일 반복을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthWeekDayRepetition
                                                                      {
                                                                          Position = OrdinalNumber.First,
                                                                          WeekDay = DayOfWeek.Sunday,
                                                                          RepetitionInterval = 2
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 2, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);
project.Save(OutDir + "CanAddRecurringTask_Months_WeekDay_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [ByMonthWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


