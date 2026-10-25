---
title: "CalendarException.MonthPosition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CalendarException 속성. 월 내에서 월 항목의 위치를 가져오거나 설정합니다."
type: docs
weight: 90
url: /ko/net/aspose.tasks/calendarexception/monthposition/
---
## CalendarException.MonthPosition property

월 내에서 월 항목의 위치를 가져오거나 설정합니다.

```csharp
public MonthPosition MonthPosition { get; set; }
```

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

* enum [MonthPosition](../../monthposition/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


