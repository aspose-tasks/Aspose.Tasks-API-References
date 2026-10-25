---
title: "MonthItemType 열거형"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.MonthItemType 열거형. 예외 반복이 예약된 월 항목을 지정합니다."
type: docs
weight: 1050
url: /ko/net/aspose.tasks/monthitemtype/
---
## MonthItemType enumeration

예외 반복이 예약된 월 항목을 지정합니다.

```csharp
public enum MonthItemType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `-1` | 정의되지 않은 월 항목 유형을 나타냅니다. |
| Day | `0` | 일 월 항목 유형을 나타냅니다. |
| Weekday | `1` | 주중 월 항목 유형을 나타냅니다. |
| WeekendDay | `2` | 주말 월 항목 유형을 나타냅니다. |
| Sunday | `3` | 일요일 월 항목 유형을 나타냅니다. |
| Monday | `4` | 월요일 월 항목 유형을 나타냅니다. |
| Tuesday | `5` | 화요일 월 항목 유형을 나타냅니다. |
| Wednesday | `6` | 수요일 월 항목 유형을 나타냅니다. |
| Thursday | `7` | 목요일 월 항목 유형을 나타냅니다. |
| Friday | `8` | 금요일 월 항목 유형을 나타냅니다. |
| Saturday | `9` | 토요일 월 항목 유형을 나타냅니다. |

## 예제

월 일별로 캘린더 예외를 정의하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// 캘린더를 생성합니다.
var calendar = project.Calendars.Add("Calendar1");

// 매 금요일에 대한 캘린더 예외를 생성합니다.
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// aa 금요일이 예외인지 확인합니다.
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// 예외를 캘린더에 추가합니다
calendar.Exceptions.Add(exception);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


