---
title: "CalendarException.Occurrences"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarException 속성. 캘린더 예외가 유효한 발생 횟수를 가져오거나 설정합니다."
type: docs
weight: 110
url: /ko/net/aspose.tasks/calendarexception/occurrences/
---
## CalendarException.Occurrences property

캘린더 예외가 유효한 발생 횟수를 가져오거나 설정합니다.

```csharp
public int Occurrences { get; set; }
```

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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


