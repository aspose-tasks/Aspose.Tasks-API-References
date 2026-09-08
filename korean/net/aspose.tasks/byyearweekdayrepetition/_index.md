---
title: "클래스 ByYearWeekDayRepetition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ByYearWeekDayRepetition 클래스. 월 내 요일의 위치를 기반으로 하는 패턴을 나타냅니다."
type: docs
weight: 200
url: /ko/net/aspose.tasks/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition class

월 내 요일의 위치를 기반으로 하는 패턴을 나타냅니다.

```csharp
public class ByYearWeekDayRepetition : YearlyRepetitionBase
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ByYearWeekDayRepetition](byyearweekdayrepetition/)() | `ByYearWeekDayRepetition` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Month](../../aspose.tasks/byyearweekdayrepetition/month/) { get; set; } | 작업이 반복되어야 하는 월을 가져오거나 설정합니다. |
| [Position](../../aspose.tasks/byyearweekdayrepetition/position/) { get; set; } | 작업이 반복되어야 하는 월의 주 중 요일 위치를 가져오거나 설정합니다. |
| [WeekDay](../../aspose.tasks/byyearweekdayrepetition/weekday/) { get; set; } | 작업이 반복되어야 하는 요일 유형을 가져오거나 설정합니다. |

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

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


