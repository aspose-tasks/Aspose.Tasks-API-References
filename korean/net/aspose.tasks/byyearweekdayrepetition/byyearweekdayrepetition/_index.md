---
title: "ByYearWeekDayRepetition.ByYearWeekDayRepetition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ByYearWeekDayRepetition 생성자. ByYearWeekDayRepetition 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/byyearweekdayrepetition/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition constructor

새 인스턴스를 초기화합니다 [`ByYearWeekDayRepetition`](../) 클래스.

```csharp
public ByYearWeekDayRepetition()
```

## 예제

새 반복 작업을 생성하면서 연도 요일 반복을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearWeekDayRepetition
                                                                      {
                                                                          Month = Month.July, WeekDay = DayOfWeek.Sunday, Position = OrdinalNumber.First
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 31, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearWeekDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


