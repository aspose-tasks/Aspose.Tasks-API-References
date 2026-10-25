---
title: "열거형 TimeUnitType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TimeUnitType 열거형. 시간 단위의 유형을 지정합니다"
type: docs
weight: 2570
url: /ko/net/aspose.tasks/timeunittype/
---
## TimeUnitType enumeration

시간 단위 유형을 지정합니다.

```csharp
public enum TimeUnitType : sbyte
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `-1` | 정의되지 않은 값을 나타내며, 해당 필드가 원본 프로젝트 파일에 정의되지 않았음을 의미합니다. |
| Minute | `0` | 분 시간 단위 유형을 나타냅니다. |
| ElapsedMinute | `1` | 경과된 분 시간 단위 유형을 나타냅니다. |
| Hour | `2` | 시간 단위 유형을 나타냅니다. |
| ElapsedHour | `3` | 경과된 시간 단위 유형을 나타냅니다. |
| Day | `4` | 일 단위 유형을 나타냅니다. |
| ElapsedDay | `5` | 경과된 일 단위 유형을 나타냅니다. |
| Week | `6` | 주 단위 유형을 나타냅니다. |
| ElapsedWeek | `7` | 경과된 주 단위 유형을 나타냅니다. |
| Month | `8` | 월 단위 유형을 나타냅니다. |
| ElapsedMonth | `9` | 경과된 월 단위 유형을 나타냅니다. |
| Percent | `10` | 백분율 시간 단위 유형을 나타냅니다. |
| ElapsedPercent | `11` | 경과된 백분율 시간 단위 유형을 나타냅니다. |
| Null | `12` | Null 시간 단위 유형을 나타냅니다. |
| MinuteEstimated | `13` | 분 예상 시간 단위 유형을 나타냅니다. |
| ElapsedMinuteEstimated | `14` | 경과된 분 예상 시간 단위 유형을 나타냅니다. |
| HourEstimated | `15` | 시간 예상 시간 단위 유형을 나타냅니다. |
| ElapsedHourEstimated | `16` | 경과된 시간 예상 시간 단위 유형을 나타냅니다. |
| DayEstimated | `17` | 일 예상 시간 단위 유형을 나타냅니다. |
| ElapsedDayEstimated | `18` | 경과된 일 예상 시간 단위 유형을 나타냅니다. |
| WeekEstimated | `19` | 주 예상 시간 단위 유형을 나타냅니다. |
| ElapsedWeekEstimated | `20` | 경과된 주 예상 시간 단위 유형을 나타냅니다. |
| MonthEstimated | `21` | 월 예상 시간 단위 유형을 나타냅니다. |
| ElapsedMonthEstimated | `22` | 경과된 월 예상 시간 단위 유형을 나타냅니다. |
| PercentEstimated | `23` | 백분율 예상 시간 단위 유형을 나타냅니다. |
| ElapsedPercentEstimated | `24` | 경과된 백분율 추정 시간 단위 유형을 나타냅니다. |
| Year | `25` | 연도 시간 단위 유형을 나타냅니다. |

## 비고

XML로 내보내는 동안 Undefined 값은 결과 XML에서 제거됩니다.

## 예제

기간을 다양한 시간 단위 유형으로 변환하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// 작업을 가져와 다양한 형식으로 기간을 계산합니다.
var task = project.RootTask.Children.GetById(1);

// 분, 일, 시간, 주 및 월 단위의 기간을 가져옵니다.
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


