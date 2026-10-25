---
title: "CalendarException.EnteredByOccurrences"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarException 속성. 반복 범위가 발생 횟수 입력으로 정의되는지 여부를 나타내는 값을 가져오거나 설정합니다. False는 반복 범위가 종료 날짜 입력으로 정의됨을 지정합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/calendarexception/enteredbyoccurrences/
---
## CalendarException.EnteredByOccurrences property

반복 범위가 발생 횟수 입력으로 정의되는지 여부를 가져오거나 설정합니다. False는 반복 범위가 종료 날짜 입력으로 정의된다는 것을 지정합니다.

```csharp
public bool EnteredByOccurrences { get; set; }
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


