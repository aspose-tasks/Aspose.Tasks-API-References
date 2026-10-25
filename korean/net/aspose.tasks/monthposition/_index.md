---
title: "열거형 MonthPosition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.MonthPosition 열거형. 월 내 항목의 위치를 지정합니다."
type: docs
weight: 1070
url: /ko/net/aspose.tasks/monthposition/
---
## MonthPosition enumeration

월 내에서 월 항목의 위치를 지정합니다.

```csharp
public enum MonthPosition
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `-1` | 정의되지 않은 월 위치를 나타냅니다. |
| First | `0` | 첫 번째 위치 월 위치를 나타냅니다. |
| Second | `1` | 두 번째 위치 월 위치를 나타냅니다. |
| Third | `2` | 세 번째 위치 월 위치를 나타냅니다. |
| Fourth | `3` | 네 번째 위치의 월 위치를 나타냅니다. |
| Last | `4` | 마지막 위치의 월 위치를 나타냅니다. |

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


