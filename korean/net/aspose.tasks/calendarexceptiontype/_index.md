---
title: "열거형 CalendarExceptionType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.CalendarExceptionType 열거형. 캘린더 예외 유형을 지정합니다."
type: docs
weight: 270
url: /ko/net/aspose.tasks/calendarexceptiontype/
---
## CalendarExceptionType enumeration

캘린더 예외 유형을 지정합니다.

```csharp
public enum CalendarExceptionType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Daily | `0` | 일일 예외 유형을 나타냅니다. |
| YearlyByDay | `1` | 월의 일에 따른 연간 예외 유형을 나타냅니다. |
| YearlyByPosition | `2` | 위치에 따른 연간 예외 유형을 나타냅니다. |
| MonthlyByDay | `3` | 월의 일에 따른 월간 예외 유형을 나타냅니다. |
| MonthlyByPosition | `4` | 위치에 따른 월간 예외 유형을 나타냅니다. |
| Weekly | `5` | 주간 예외 유형을 나타냅니다. |
| ByDayCount | `6` | 일 수에 따른 예외 유형을 나타냅니다. |
| ByWeekDayCount | `7` | 요일 수에 따른 예외 유형을 나타냅니다. |
| NoExceptionType | `8` | 예외 유형이 없음을 나타냅니다. |

## 예제

발생 횟수로 캘린더 예외를 정의하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 캘린더 정의
var calendar = project.Calendars.Add("Calendar1");

// 예외를 정의하고 발생 횟수를 지정합니다.
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// 캘린더에 예외를 추가합니다.
calendar.Exceptions.Add(exception);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


